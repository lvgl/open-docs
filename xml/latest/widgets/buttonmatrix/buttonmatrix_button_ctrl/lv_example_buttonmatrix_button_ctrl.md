```xml title="examples/widgets/buttonmatrix/buttonmatrix_button_ctrl/lv_example_buttonmatrix_button_ctrl.xml" source="https://github.com/lvgl/lvgl/blob/f92d9d2829dd66417588a4e4199bc46060d4e67b/examples/widgets/buttonmatrix/buttonmatrix_button_ctrl/lv_example_buttonmatrix_button_ctrl.xml"
<!--
 @title Button matrix per-button control flags
 @brief Apply checkable, checked, disabled, and hidden flags via `ctrl_map`.

 Each token in `ctrl_map` is a `|`-separated list of flag names that applies to
 the matching button in `map`. The four buttons here show a plain button, a
 checkable button that starts checked (`checkable|checked`), a `disabled` button,
 and a `hidden` button which still reserves its slot in the layout.
-->
<screen>
	<view>
		<!-- 💡 Edit individual `ctrl_map` tokens to see how each button state is rendered and which still receives input. -->
		<!-- One row with four differently-flagged buttons -->
		<lv_buttonmatrix name="buttonmatrix"
			align="center"
			width="90%"
			height="60"
			map="'Normal' 'Checked' 'Disabled' 'Hidden'"
			ctrl_map="none checkable|checked disabled hidden"
		/>
	</view>
</screen>
```
