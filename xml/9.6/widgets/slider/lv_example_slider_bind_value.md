```xml title="examples/widgets/slider/lv_example_slider_bind_value.xml" source="https://github.com/lvgl/lvgl/blob/9242b9f317c551cc0b06ad3bebc2c12f37291a97/examples/widgets/slider/lv_example_slider_bind_value.xml"
<!--
 @title Slider bind value
 @brief Two-way bind a slider to a shared int subject; a label mirrors the live value.

 `subject_value` lives in `examples/xml_project/globals.xml` (range 0..100, default 50).
 The slider's `bind_value` reads and writes the subject: dragging it pushes the new
 value out so anything else bound to `subject_value` (here, the label) updates
 immediately. `bind_text-fmt` lets a label render a numeric subject through a
 printf-style format.
-->
<screen>
	<view flex_flow="column" style_flex_main_place="center" style_flex_cross_place="center" style_flex_track_place="center" style_pad_row="16">
		<!-- 💡 Drag the slider; the label re-renders because both widgets share `subject_value`. -->
		<lv_slider name="slider" width="90%" bind_value="subject_value" />

		<lv_label name="label" bind_text="subject_value" bind_text-fmt="Value: %d/100" />
	</view>
</screen>
```
