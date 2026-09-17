```xml title="examples/get_started/get_started_hello_world/lv_example_get_started_hello_world.xml" source="https://github.com/lvgl/lvgl/blob/0e919db876e4c414019877d990c01d5a47966955/examples/get_started/get_started_hello_world/lv_example_get_started_hello_world.xml"
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
