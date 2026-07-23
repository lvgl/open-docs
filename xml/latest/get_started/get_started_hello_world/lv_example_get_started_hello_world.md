```xml title="examples/get_started/get_started_hello_world/lv_example_get_started_hello_world.xml" source="https://github.com/lvgl/lvgl/blob/c4424b27d63db752aa75f9fdffe30c6467b55ad1/examples/get_started/get_started_hello_world/lv_example_get_started_hello_world.xml"
<!--
 @title Hello world label
 @brief Paint the screen background and center a label on it.

 The view sets its own `style_bg_color` to a dark teal and `style_text_color`
 to white. The label sets no color of its own — it inherits white from the
 view — and `align="center"` places it in the middle of the display.
-->
<screen>
	<view style_bg_color="0x003a57" style_text_color="0xffffff">
		<lv_label name="label" align="center" text="Hello world" />
	</view>
</screen>
```
