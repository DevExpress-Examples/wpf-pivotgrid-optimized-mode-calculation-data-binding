<!-- default file list -->
*Files to look at*:
* [MainWindow.xaml](./CS/PivotGridOptimizedModeExample/MainWindow.xaml)
<!-- default file list end -->

# Pivot Grid Optimized Mode - Field Calculation Data Binding

This example demonstrates how to use a **Data Binding API** to specify the PivotGridField's data source. Instead of bound and unbound fields, the Data Binding API allows you to specify the data binding source. The former _bound_ field gets data from a data source column - the  _bound_ field is a field bound to data with the  **DataSourceColumnBinding** instance. The former _unbound_ fields are fields that get data from calculations (**ExpressionDataBinding**), specific window calculations (**RunningTotalBinding**, **MovingCalculationBinding** and others), or from a window calculation specified by an expression (**WindowExpressionBinding**).

The **Data Binding API** is in effect only in the [Optimized Mode](https://docs.devexpress.com/CoreLibraries/DevExpress.XtraPivotGrid.PivotDataProcessingEngine). Other calculation engines ignore the [PivotGridField.DataBinding](http://docs.devexpress.devx/WPF/DevExpress.Xpf.PivotGrid.PivotGridField.DataBinding) property.

![](/images/screenshot.png)

> The project uses the [ExcelDataSource](https://docs.devexpress.com/CoreLibraries/DevExpress.DataAccess.Excel.ExcelDataSource) component in the **ExcelItemsSource** wrapper. It requires references to the following assemblies in addition to references created automatically when the PivotGrid control is dropped from the Toolbox:
> * DevExpress.DataAccess
> * DevExpress.Xpf.Core.Extensions
> * DevExpress.Xpf.Grid
> * DevExpress.Xpf.Grid.Core

**See also:**

* [Optimized Calculation Engine](https://docs.devexpress.com/CoreLibraries/401367)