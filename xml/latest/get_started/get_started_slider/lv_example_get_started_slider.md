```xml title="examples/get_started/get_started_slider/lv_example_get_started_slider.xml" source="https://github.com/lvgl/lvgl/blob/c51feccbd7a602d48bc9e535e8dab7f9bc01df74/examples/get_started/get_started_slider/lv_example_get_started_slider.xml"
<!--
 @title Slider with live value
 @brief Mirror a slider's value into a label through a shared subject.

 The slider writes its position to `subject_value` with `bind_value`, and the
 label reads the same subject with `bind_text` + `bind_text-fmt="%d"`. Because
 both refer to one subject, dragging the slider updates the label with no event
 callback — the binding keeps the two in sync.
-->
<screen>
	<view>
		<!-- 💡 Drag the slider; the label tracks it because both share `subject_value`. -->
		<lv_label name="label" align="center" y="-20" bind_text="subject_value" bind_text-fmt="%d" />
		<lv_slider name="slider" align="center" y="20" width="90%" bind_value="subject_value" />
	</view>
</screen>
```
