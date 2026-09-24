```xml title="examples/widgets/label/lv_example_label_bind_text.xml" source="https://github.com/lvgl/lvgl/blob/c526cd81f316e59a582e32f073e57cae182cf410/examples/widgets/label/lv_example_label_bind_text.xml"
<!--
 @title Label bind text
 @brief Bind a label to a string subject; buttons rewrite the subject on click.

 `subject_text` is a string subject from `examples/xml_project/globals.xml`. The
 label uses `bind_text` to listen for changes. Each button carries a
 `<subject_set_string_event>` child that, on click, writes a fixed value into
 `subject_text` — and the label re-renders automatically.
-->
<screen>
	<view>
		<!-- 💡 Click either button; the label updates because it reads `subject_text` live. -->
		<lv_label name="label_1" bind_text="subject_text" align="center" y="-50" />

		<lv_button name="button_1" align="center">
			<lv_label name="label_2" align="center" text="Idle" />
			<subject_set_string_event subject="subject_text" value="Idle" />
		</lv_button>
		<lv_button name="button_2" align="center" y="50">
			<lv_label name="label_3" align="center" text="Running" />
			<subject_set_string_event subject="subject_text" value="Running" />
		</lv_button>
	</view>
</screen>
```
