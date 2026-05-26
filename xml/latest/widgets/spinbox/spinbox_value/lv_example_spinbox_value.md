```xml title="examples/widgets/spinbox/spinbox_value/lv_example_spinbox_value.xml" source="https://github.com/lvgl/lvgl/blob/99df9b9ac7b096ca30802f8d3a12452b78bc9110/examples/widgets/spinbox/spinbox_value/lv_example_spinbox_value.xml"
<!--
 @title Spinbox value, range, and step
 @brief Pin the initial value, clamp it to a numeric range, and set the per-step delta.

 `value` is the starting number shown in the spinbox. `min_value`/`max_value`
 clamp every adjustment — pressing the increment past the maximum stays at
 the maximum. `step` is how much each key/press changes the value. With
 `rollover="false"` (the default) the value sticks at the bounds; see
 `spinbox_rollover` for the wraparound variant.
-->
<screen>
	<view flex_flow="column" style_flex_main_place="center" style_flex_cross_place="center" style_flex_track_place="center" style_pad_row="16">
		<!-- 💡 Edit `step` to 5 or 10; each press now changes by that delta until a bound is hit. -->
		<lv_spinbox name="spinbox" width="160"
			digit_count="3"
			value="25"
			min_value="0" max_value="100"
			step="1" />
	</view>
</screen>
```
