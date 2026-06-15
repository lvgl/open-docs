```xml title="examples/widgets/switch/lv_example_switch_orientation.xml" source="https://github.com/lvgl/lvgl/blob/603d534270624e7d3f37f70cdd5f608a41825305/examples/widgets/switch/lv_example_switch_orientation.xml"
<!--
 @title Switch orientation
 @brief Lay the switch out horizontally or vertically.

 `orientation="auto"` (the default) picks horizontal when the widget is
 wider than it is tall, and vertical otherwise. Forcing the orientation with
 `horizontal` or `vertical` overrides this — useful when the layout
 dimensions don't match the orientation you want, e.g. a tall vertical
 switch inside a wide row.
-->
<screen>
	<view flex_flow="row" style_flex_main_place="space_evenly" style_flex_cross_place="center" style_flex_track_place="center">
		<!-- 💡 Swap `orientation` on either switch to compare auto-derived vs explicit layouts. -->

		<lv_switch name="sw_1" width="60" height="30" orientation="horizontal" checked="true" />
		<lv_switch name="sw_2" width="30" height="60" orientation="vertical" checked="true" />
	</view>
</screen>
```
