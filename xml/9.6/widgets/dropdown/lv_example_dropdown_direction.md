```xml title="examples/widgets/dropdown/lv_example_dropdown_direction.xml" source="https://github.com/lvgl/lvgl/blob/5d0e67b01d5f6d6d3f1e49a544b0f65e36075e73/examples/widgets/dropdown/lv_example_dropdown_direction.xml"
<!--
 @title Dropdown open direction
 @brief Open the option list towards a specific edge.

 Four dropdowns sit on the four sides of the screen and use the dir attribute to choose
 which way their option list pops. The default is bottom, but top, left, and right are
 useful when a dropdown sits close to a screen edge and there is no room to expand
 downward.
-->
<screen>
	<view>
		<!-- 💡 Click each dropdown: each list pops toward the screen edge defined by its dir attribute. -->
		<!-- Default: list opens downward -->
		<lv_dropdown name="dropdown_1" align="top_mid" y="20" options="Apple&#10;Banana&#10;Orange&#10;Melon" />

		<!-- List opens upward -->
		<lv_dropdown
			name="dropdown_2"
			align="bottom_mid"
			y="-20"
			dir="top"
			options="Apple&#10;Banana&#10;Orange&#10;Melon"
		/>

		<!-- List opens to the right -->
		<lv_dropdown
			name="dropdown_3"
			align="left_mid"
			x="20"
			width="80"
			dir="right"
			options="Apple&#10;Banana&#10;Orange&#10;Melon"
		/>

		<!-- List opens to the left -->
		<lv_dropdown
			name="dropdown_4"
			align="right_mid"
			x="-20"
			width="80"
			dir="left"
			options="Apple&#10;Banana&#10;Orange&#10;Melon"
		/>
	</view>
</screen>
```
