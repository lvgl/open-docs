```xml title="examples/widgets/keyboard/keyboard_modes/lv_example_keyboard_modes.xml" source="https://github.com/lvgl/lvgl/blob/829c7a22191e5dc0aceba71c54c09f42c08e3ac5/examples/widgets/keyboard/keyboard_modes/lv_example_keyboard_modes.xml"
<!--
 @title Keyboard modes
 @brief Switch between text and number layouts via the `mode` attribute.

 `mode` selects the keymap LVGL shows. `text_lower`/`text_upper` give the
 letter layouts with case shift keys; `special` swaps in punctuation;
 `number` shows the calculator-style numeric pad. The mode persists until
 changed — pressing the in-layout `ABC`/`abc`/`1#` keys switches the keymap
 at runtime, while this attribute pins the initial layout.
-->
<screen>
	<view>
		<!-- 💡 Change `mode` from `number` to `text_lower`, `text_upper`, or `special` to see each keymap. -->
		<lv_textarea name="textarea" align="top_mid" y="10" width="90%" height="60"
			one_line="true" placeholder_text="Numbers only" />

		<lv_keyboard name="keyboard" align="bottom_mid" width="100%" height="50%"
			mode="number" />
	</view>
</screen>
```
