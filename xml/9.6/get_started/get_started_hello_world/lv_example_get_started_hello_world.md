```xml title="examples/get_started/get_started_hello_world/lv_example_get_started_hello_world.xml" source="https://github.com/lvgl/lvgl/blob/200ac28a72e4337b56d73e4c48bfd661ea9ec041/examples/get_started/get_started_hello_world/lv_example_get_started_hello_world.xml"
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
