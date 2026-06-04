```xml title="examples/widgets/tabview/lv_example_tabview_basic.xml" source="https://github.com/lvgl/lvgl/blob/3f9b6f6323a47bc7a7b8ad9c37047c16fe182c31/examples/widgets/tabview/lv_example_tabview_basic.xml"
<!--
 @title Tab view basic structure
 @brief Three tabs hosting plain labels, demonstrating the minimal markup.

 An `lv_tabview` carries three `lv_tabview-tab` children. The `text` arg sets
 each tab's button caption and the children of a tab become its content. No
 `tab_bar_position` or `active` is set, so the bar sits on the top edge and
 the first tab opens.
-->
<screen>
	<view>
		<!-- 💡 Tap a tab button or swipe horizontally to switch tabs. -->
		<lv_tabview name="tabview" width="100%" height="100%">
			<lv_tabview-tab text="Tab 1">
				<lv_label name="label_1" align="center" text="First tab" />
			</lv_tabview-tab>
			<lv_tabview-tab text="Tab 2">
				<lv_label name="label_2" align="center" text="Second tab" />
			</lv_tabview-tab>
			<lv_tabview-tab text="Tab 3">
				<lv_label name="label_3" align="center" text="Third tab" />
			</lv_tabview-tab>
		</lv_tabview>
	</view>
</screen>
```
