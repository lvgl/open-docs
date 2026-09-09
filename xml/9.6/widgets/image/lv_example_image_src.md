```xml title="examples/widgets/image/lv_example_image_src.xml" source="https://github.com/lvgl/lvgl/blob/db53672c9dfe1eadf2b2c7382a02ea107992ef09/examples/widgets/image/lv_example_image_src.xml"
<!--
 @title Image source
 @brief Display an image registered globally for the project.

 `lv_image` paints whatever is set as its `src`.
 In C the image can be a file or a C array.
 In XML the source needs to b set in globals.xml.-->
<screen>
	<view>
		<!-- 💡 Register another image in `globals.xml` and swap `src` to its name to see a different bitmap. -->
		<lv_image name="image" src="img_example_lvgl_logo" align="center" />
	</view>
</screen>
```
