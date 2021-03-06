---
title: Week Column
page_title: Week Column | Telerik UI MultiViewCalendar HtmlHelper for ASP.NET MVC
description: "Render a column displaying the number of the weeks within the current month view when working with the Telerik UI MultiViewCalendar."
slug: week_column_multiviewcalendar_aspnetmvc
position: 7
---

# Week Column

In the MultiViewCalendar, you can render a column which displays the number of the weeks within the current `month` view.

```ASPX

        <%: Html.Kendo().MultiViewCalendar()
            .Name("MultiViewCalendar")
            .WeekNumber(true)
        %>
```
```Razor

        @(Html.Kendo().MultiViewCalendar()
            .Name("MultiViewCalendar")
            .WeekNumber(true)
        )
```

## See Also

* [Week Column in the MultiViewCalendar HtmlHelper for ASP.NET MVC (Demo)](https://demos.telerik.com/aspnet-mvc/multiviewcalendar/week-column)
* [Server-Side API](/api/multiviewcalendar)
