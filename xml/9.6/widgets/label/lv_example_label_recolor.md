```xml title="examples/widgets/label/lv_example_label_recolor.xml" source="https://github.com/lvgl/lvgl/blob/1df2741e706b5a98ae9bebe324ddf0d4d4a17e89/examples/widgets/label/lv_example_label_recolor.xml"
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
