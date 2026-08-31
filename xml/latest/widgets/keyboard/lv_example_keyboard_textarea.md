```xml title="examples/widgets/keyboard/lv_example_keyboard_textarea.xml" source="https://github.com/lvgl/lvgl/blob/0de12499ea17924486fe9ec1f6050898cdd9b947/examples/widgets/keyboard/lv_example_keyboard_textarea.xml"
<!--
 @title Keyboard with text area
 @brief Pair a keyboard with a textarea so typed keys land in the field.

 The keyboard and the textarea sit on the same screen; LVGL's default focus
 group routes key presses to whichever input widget currently holds focus
 (here the textarea is the only one). In runtime code you'd usually call
 `lv_keyboard_set_textarea(kb, ta)` to pin the link explicitly, but for a
 single textarea on a screen the default group is sufficient.
-->
<screen>
	<view>
		<!-- 💡 Tap the textarea to focus it, then type — the keyboard writes into the focused input. -->
		<lv_textarea
			name="textarea"
			align="top_mid"
			y="10"
			width="90%"
			one_line="true"
			placeholder_text="Type here..."
		/>

		<lv_keyboard name="keyboard" align="bottom_mid" width="100%" height="60%" mode="text_lower" />
	</view>
</screen>
```
