```xml title="examples/widgets/buttonmatrix/buttonmatrix_one_checked/lv_example_buttonmatrix_one_checked.xml" source="https://github.com/lvgl/lvgl/blob/18760b7f0312f8a7e13147f2ca83cd10710438c1/examples/widgets/buttonmatrix/buttonmatrix_one_checked/lv_example_buttonmatrix_one_checked.xml"
<!--
 @title Button matrix one-checked mode
 @brief Make the matrix behave like a radio group with a single checked button.

 With `one_checked="true"`, the buttons that carry `checkable` in `ctrl_map` form
 a mutually exclusive group: pressing one un-checks the previously checked button.
 Every weekday here is `checkable`, and Tue starts as `checkable|checked` so the
 example doubles as a small weekday selector.
-->
<screen>
	<view>
		<!-- 💡 Tap any day: it becomes checked and the previously checked button clears automatically. -->
		<!-- Weekday selector with single-checked semantics -->
		<lv_buttonmatrix name="buttonmatrix"
			align="center"
			width="90%"
			height="60"
			one_checked="true"
			map="'Mon' 'Tue' 'Wed' 'Thu' 'Fri'"
			ctrl_map="checkable checkable|checked checkable checkable checkable"
		/>
	</view>
</screen>
```
