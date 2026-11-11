```xml title="examples/widgets/dropdown/lv_example_dropdown_text.xml" source="https://github.com/lvgl/lvgl/blob/53819fe4fd3f3a767420743cbfdb2816f3928931/examples/widgets/dropdown/lv_example_dropdown_text.xml"
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
