```xml title="examples/widgets/textarea/lv_example_textarea_placeholder.xml" source="https://github.com/lvgl/lvgl/blob/bb8ef34b1328006eecc4d192c9f45a04e54de31d/examples/widgets/textarea/lv_example_textarea_placeholder.xml"
<!--
 @title Text area placeholder
 @brief Show a hint while the text area is empty.

 Both text areas carry the same `placeholder_text`. The first is left empty
 so the grey hint is visible; the second has `text` set, which hides the
 placeholder — the contrast shows exactly when the hint appears.
-->
<screen>
	<view
		flex_flow="column"
		style_flex_main_place="center"
		style_flex_cross_place="center"
		style_flex_track_place="center"
		style_pad_row="16"
	>
		<!-- 💡 The placeholder only shows while the field is empty; typing replaces it. -->
		<!-- Empty: placeholder hint is shown -->
		<lv_textarea name="textarea_1" width="60%" one_line="true" placeholder_text="Search..." />

		<!-- Filled: placeholder is hidden -->
		<lv_textarea name="textarea_2" width="60%" one_line="true" placeholder_text="Search…" text="Hello world!" />
	</view>
</screen>
```
