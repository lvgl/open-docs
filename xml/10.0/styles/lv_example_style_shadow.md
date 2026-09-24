```xml title="examples/styles/lv_example_style_shadow.xml" source="https://github.com/lvgl/lvgl/blob/c526cd81f316e59a582e32f073e57cae182cf410/examples/styles/lv_example_style_shadow.xml"
<!--
 @title Box shadow
 @brief Lift a card off the page with a soft, offset shadow.

 `shadow_width="30"` sets the blur and `shadow_color` tints it.
 `shadow_offset_y="12"` drops the shadow below the card so it reads as
 elevation, and `shadow_opa="80"` keeps it soft. With both offsets at 0
 the same blur becomes an even glow instead.
-->
<screen>
	<styles>
		<!-- Soft indigo elevation shadow under a clean card -->
		<style
			name="style_elevated"
			radius="20"
			bg_opa="100%"
			bg_color="0xffffff"
			border_width="0"
			shadow_color="0x312e81"
			shadow_width="30"
			shadow_offset_y="12"
			shadow_opa="80"
		/>
	</styles>

	<view>
		<!-- 💡 Set `shadow_offset_x`/`shadow_offset_y` to 0 to turn the elevation into an even glow. -->
		<lv_obj name="container" align="center" width="210" height="130">
			<style name="style_elevated" />
			<lv_label name="label" align="center" text="Elevated" />
		</lv_obj>
	</view>
</screen>
```
