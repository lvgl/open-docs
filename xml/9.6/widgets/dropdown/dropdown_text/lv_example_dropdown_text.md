```xml title="examples/widgets/dropdown/dropdown_text/lv_example_dropdown_text.xml" source="https://github.com/lvgl/lvgl/blob/18760b7f0312f8a7e13147f2ca83cd10710438c1/examples/widgets/dropdown/dropdown_text/lv_example_dropdown_text.xml"
<!--
 @title Dropdown fixed text
 @brief Pin the dropdown button label regardless of selection.

 Without a text attribute the dropdown shows the currently selected option (left). With
 text="Menu" the button always displays that string while the option list remains
 intact, which is useful for icon-style or fixed-label menus.
-->
<screen>
	<view>
		<!-- 💡 Set text to make the button always show that fixed label, regardless of which option is picked. -->
		<!-- Without text the button reflects the selected option -->
		<lv_dropdown name="dropdown_1" align="left_mid" x="14" width="110" options="Cut&#10;Copy&#10;Paste" />

		<!-- text='Menu' overrides the displayed option -->
		<lv_dropdown name="dropdown_2" align="right_mid" x="-14" width="110" text="Menu" options="Cut&#10;Copy&#10;Paste" />
	</view>
</screen>
```
