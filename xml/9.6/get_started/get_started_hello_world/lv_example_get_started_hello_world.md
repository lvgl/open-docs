```xml title="examples/get_started/get_started_hello_world/lv_example_get_started_hello_world.xml" source="https://github.com/lvgl/lvgl/blob/b6d1bb48834295f9c1086136bcb7b5f5c41b90ec/examples/get_started/get_started_hello_world/lv_example_get_started_hello_world.xml"
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
