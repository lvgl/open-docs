```xml title="examples/widgets/buttonmatrix/buttonmatrix_popover/lv_example_buttonmatrix_popover.xml" source="https://github.com/lvgl/lvgl/blob/180adf91d757e1a895170564fddd15d4a891c86c/examples/widgets/buttonmatrix/buttonmatrix_popover/lv_example_buttonmatrix_popover.xml"
<!--
 @title Button matrix popover preview
 @brief Show a magnified label above a button while it is pressed.

 The `popover` flag mirrors the on-screen keyboard convention: while a button is
 held down, its text floats up in a small popover above the finger so the user
 can still read what they are pressing. The entire top row carries `popover` in
 `ctrl_map`, which is how a keyboard layer typically enables the feature.
-->
<screen>
	<view>
		<!-- 💡 Press and hold any letter: a popover appears above the pressed key while the press is active. -->
		<!-- Keyboard-style row with popover enabled on every button -->
		<lv_buttonmatrix name="buttonmatrix"
			align="center"
			width="90%"
			height="60"
			map="'Q' 'W' 'E' 'R' 'T' 'Y'"
			ctrl_map="popover popover popover popover popover popover"
		/>
	</view>
</screen>
```
