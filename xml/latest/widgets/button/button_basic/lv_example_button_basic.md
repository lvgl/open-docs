```xml title="examples/widgets/button/button_basic/lv_example_button_basic.xml" source="https://github.com/lvgl/lvgl/blob/77b321d3ae1a7d239ce373f77d08a144cc8b3f2f/examples/widgets/button/button_basic/lv_example_button_basic.xml"
<!--
 @title Button basics
 @brief Two buttons showing default content-sized sizing and an explicit width.

 The first button uses default sizing so it wraps tightly around its label. The second
 button sets an explicit width and height, illustrating that a button is just a
 clickable base widget with a label child.
-->
<screen>
	<view flex_flow="column" style_flex_main_place="center" style_flex_cross_place="center" style_flex_track_place="center" style_pad_row="16">
		<!-- 💡 Resize one button or change its label to see how content-sizing reacts. -->
		<!-- Default size driven by label content -->
		<lv_button name="button_1">
			<lv_label name="label_1" align="center" text="Click me" />
		</lv_button>

		<!-- Explicit width and height -->
		<lv_button name="button_2" width="160" height="48">
			<lv_label name="label_2" align="center" text="Wide button" />
		</lv_button>
	</view>
</screen>
```
