```xml title="examples/widgets/dropdown/lv_example_dropdown_text.xml" source="https://github.com/lvgl/lvgl/blob/1df2741e706b5a98ae9bebe324ddf0d4d4a17e89/examples/widgets/dropdown/lv_example_dropdown_text.xml"
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
		<lv_dropdown name="dropdown_1" align="center" x="-100" width="110" options="Cut&#10;Copy&#10;Paste" />

		<!-- text='Menu' overrides the displayed option -->
		<lv_dropdown
			name="dropdown_2"
			align="center"
			x="100"
			width="110"
			text="Menu"
			options="Cut&#10;Copy&#10;Paste"
		/>
	</view>
</screen>
```
