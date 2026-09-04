```xml title="examples/widgets/tabview/lv_example_tabview_tab_bar_position.xml" source="https://github.com/lvgl/lvgl/blob/3f8302923d8ed252a013cc9f79824a4005986445/examples/widgets/tabview/lv_example_tabview_tab_bar_position.xml"
<!--
 @title Tab view tab bar position
 @brief Place the tab bar on any of the four sides.

 Four mini tab views lay out a 2×2 grid covering every `tab_bar_position` value:
 `top`, `bottom`, `left`, `right`. Each carries a distinct `style_bg_color` so
 the four widgets are easy to tell apart at a glance; only `tab_bar_position`
 changes the layout itself.
-->
<screen>
	<view>
		<!-- 💡 Change tab_bar_position to top/bottom/left/right to move the tab bar. -->
		<!-- Bar on the top edge -->

		<!-- Bar on the right edge -->
		<lv_tabview name="tabview_1" tab_bar_position="right" style_bg_color="0xce93d8" style_bg_opa="100%">
			<lv_tabview-tab text="A">
				<lv_label name="label_1" align="center" text="Right tab bar" />
			</lv_tabview-tab>
			<lv_tabview-tab text="B">
				<lv_label name="label_2" align="center" text="Same here" />
			</lv_tabview-tab>
		</lv_tabview>
	</view>
</screen>
```
