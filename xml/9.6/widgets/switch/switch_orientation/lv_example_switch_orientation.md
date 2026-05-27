```xml title="examples/widgets/switch/switch_orientation/lv_example_switch_orientation.xml" source="https://github.com/lvgl/lvgl/blob/180adf91d757e1a895170564fddd15d4a891c86c/examples/widgets/switch/switch_orientation/lv_example_switch_orientation.xml"
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
	<view flex_flow="row" style_flex_main_place="space_evenly" style_flex_cross_place="center" style_pad_column="32">
		<!-- 💡 Swap `orientation` on either switch to compare auto-derived vs explicit layouts. -->

		<lv_switch name="sw_1" width="60" height="30" orientation="horizontal" checked="true" />
		<lv_switch name="sw_2" width="30" height="60" orientation="vertical" checked="true" />
	</view>
</screen>
```
