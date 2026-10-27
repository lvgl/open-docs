```xml title="examples/widgets/led/lv_example_led_color.xml" source="https://github.com/lvgl/lvgl/blob/50c61a27338c1a9837d308f9a116bea78d072323/examples/widgets/led/lv_example_led_color.xml"
<!--
 @title LED color
 @brief Three LEDs lit in different hues via the color attribute.

 The color attribute sets the LED's background, border, and shadow color together, so
 a single value drives the whole lit-bulb look. Brightness stays at the default here
 to isolate the effect of changing the color alone.
-->
<screen>
	<view flex_flow="column" style_flex_main_place="center" style_flex_cross_place="center" style_flex_track_place="center" style_pad_row="16">
		<!-- 💡 Edit each color attribute to recolor that LED. -->
		<!-- Red LED -->
		<lv_led name="led_1" width="40" height="40" color="0xff3030" />

		<!-- Green LED -->
		<lv_led name="led_2" width="40" height="40" color="0x30c050" />

		<!-- Blue LED -->
		<lv_led name="led_3" width="40" height="40" color="0x3080ff" />
	</view>
</screen>
```
