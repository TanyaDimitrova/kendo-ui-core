---
title:  Ajax Binding
page_title: Ajax Binding | Telerik UI DropDownTree HtmlHelper for ASP.NET Core
description: "Learn how to implement Ajax Binding with Telerik UI DropDownTree HtmlHelper for ASP.NET Core (MVC 6 or ASP.NET Core MVC)."
slug: htmlhelpers_dropdowntree_ajaxbinding_aspnetcore
position: 2
---

# Ajax Data Binding

The DropDownTree provides support for remote data binding by using a `DataSource` configuration object.

```Razor
@(Html.Kendo().DropDownTree()
    .Name("dropdowntree")
    .DataTextField("Name")
    .DataValueField("id")
    .DataSource(dataSource => dataSource
        .Read(read => read
            .Action("Read_DropDownTreeData", "Home")
        )
    )
)
```
```Controller
public static IList<HierarchicalViewModel> GetHierarchicalData()
{
    var result = new List<HierarchicalViewModel>()
    {
        new HierarchicalViewModel() { ID = 1, ParentID = null, HasChildren = true, Name = "Parent item" },
        new HierarchicalViewModel() { ID = 2, ParentID = 1, HasChildren = true, Name = "Parent item" },
        new HierarchicalViewModel() { ID = 3, ParentID = 1, HasChildren = false, Name = "Item" },
        new HierarchicalViewModel() { ID = 4, ParentID = 2, HasChildren = false, Name = "Item" },
        new HierarchicalViewModel() { ID = 5, ParentID = 2, HasChildren = false, Name = "Item" }
    };

    return result;
}

public IActionResult Read_DropDownTreeData(int? id)
{
    var result = GetHierarchicalData()
        .Where(x => id.HasValue ? x.ParentID == id : x.ParentID == null)
        .Select(item => new {
            id = item.ID,
            Name = item.Name,
            hasChildren = item.HasChildren
        });

    return Json(result);
}
```

## See Also

* [Local Data Binding by the DropDownTree HtmlHelper for ASP.NET Core (Demo)](https://demos.telerik.com/aspnet-core/dropdowntree/local-data-binding)
* [Client-Side API](https://docs.telerik.com/kendo-ui/api/javascript/ui/dropdowntree)
* [Server-Side API](/api/dropdowntree)
