```xml title="examples/widgets/table/lv_example_table_cells.xml" source="https://github.com/lvgl/lvgl/blob/e97ca14b69d7821f709d8b9212c5e9ebf89dd116/examples/widgets/table/lv_example_table_cells.xml"
<!--
 @title Table cell values
 @brief Populate a grid of cells with text using `<lv_table-cell>` children.

 Each cell is declared with its `row`/`column` (zero-based) and a `value`
 string. Cells default to empty, so only the populated coordinates have
 visible text. `row_count`/`column_count` size the grid up front so the
 cells render in the right slots even if their declaration order doesn't
 walk row-major.
-->
<screen>
	<view>
		<!-- 💡 Add another `<lv_table-cell>` with different `row`/`column` to populate more cells. -->
		<lv_table name="table" row_count="3" column_count="2" align="center">
			<!-- Header row -->
			<lv_table-cell row="0" column="0" value="City" />
			<lv_table-cell row="0" column="1" value="Population" />
			<!-- Data rows -->
			<lv_table-cell row="1" column="0" value="Berlin" />
			<lv_table-cell row="1" column="1" value="3.7M" />
			<lv_table-cell row="2" column="0" value="Paris" />
			<lv_table-cell row="2" column="1" value="2.1M" />
		</lv_table>
	</view>
</screen>
```
