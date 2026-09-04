```xml title="examples/widgets/spinbox/lv_example_spinbox_rollover.xml" source="https://github.com/lvgl/lvgl/blob/7f137902570087f9e5d8822a5b41e94d8ce87dc6/examples/widgets/spinbox/lv_example_spinbox_rollover.xml"
<!--
 @title Spinbox rollover
 @brief Wrap the value around when it hits a bound instead of sticking.

 `rollover="true"` makes the spinbox treat its range as circular: pressing
 past `max_value` jumps to `min_value` and vice versa. This is convenient
 for cyclic quantities like hours (0..23) or angles (0..359), where the user
 should be able to step from 23 → 0 without re-entering the value.
-->
<screen>
	<view>
		<!-- 💡 Increment past 23; the value wraps to 0 because `rollover="true"`. -->
		<lv_label text="Use the arrows to change the value" align="center" y="-50" />
		<lv_spinbox
			name="spinbox"
			width="160"
			digit_count="2"
			value="22"
			min_value="0"
			max_value="23"
			step="1"
			align="center"
			rollover="true"
		/>
	</view>
</screen>
```
