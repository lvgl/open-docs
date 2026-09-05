```xml title="examples/widgets/image/lv_example_image_src.xml" source="https://github.com/lvgl/lvgl/blob/8a8fdf2baa66eb8c3d908cbddc593c255daf41d5/examples/widgets/image/lv_example_image_src.xml"
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
