```xml title="examples/widgets/label/lv_example_label_text_selection.xml" source="https://github.com/lvgl/lvgl/blob/3ec42fc4b79c8a2effa11198314c70935349a109/examples/widgets/label/lv_example_label_text_selection.xml"
<!--
 @title Label text selection range
 @brief Highlight a substring inside a label.

 text_selection_start and text_selection_end take character indices and visually highlight
 the range between them, useful for showing selected or marked-up text. The example
 highlights characters 11..16 of the label content.
-->
<screen>
	<view flex_flow="column" style_flex_main_place="center" style_flex_cross_place="center" style_flex_track_place="center" style_pad_row="16">
		<!-- 💡 Adjust text_selection_start/end to highlight different ranges in the same text. -->
		<!-- Label with predefined selected text range -->
		<lv_label name="label"
			text="Selectable text range example"
			text_selection_start="11"
			text_selection_end="16"
		/>
	</view>
</screen>
```
