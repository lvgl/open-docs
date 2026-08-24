```xml title="examples/widgets/label/lv_example_label_recolor.xml" source="https://github.com/lvgl/lvgl/blob/224c7dc61f45f7e97becf23ad629d412df35405f/examples/widgets/label/lv_example_label_recolor.xml"
<!--
 @title Label text recolor
 @brief Recolor individual words via inline color tags.

 With recolor="true", segments wrapped as "#RRGGBB ... #" render in the given color. This
 lets a single label mix multiple colors in one string without splitting it into separate
 label widgets.
-->
<screen>
	<view>
		<!-- 💡 Adjust inline #RRGGBB segments to recolor different words and ranges in one label. -->
		<!-- Recolor-enabled label using inline #RRGGBB color commands -->
		<lv_label
			name="label"
			align="center"
			recolor="true"
			text="Write a #ff0000 red# word, a #00a000 green# word, and a #0000ff blue# word."
		/>
	</view>
</screen>
```
