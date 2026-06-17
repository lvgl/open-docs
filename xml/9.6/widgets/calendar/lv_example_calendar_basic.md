```xml title="examples/widgets/calendar/lv_example_calendar_basic.xml" source="https://github.com/lvgl/lvgl/blob/d1815aa742b940cdeedee6b23025d6332913c36f/examples/widgets/calendar/lv_example_calendar_basic.xml"
<!--
 @title Calendar basics
 @brief Month view with an arrow header for navigation.

 `today_*` marks the current date (rendered with the today highlight). `shown_*`
 controls which month the calendar opens on — here we start a month behind
 today so the user immediately sees that the today indicator only fires when
 the shown month matches. A `<header_arrow/>` child adds prev/next arrows to
 the top of the calendar; swap it for `<header_dropdown/>` to get the
 month/year selector variant.
-->
<screen>
	<view>
		<!-- 💡 Tap a day to select it; use the header arrows to jump between months. -->
		<lv_calendar
			name="calendar"
			width="300"
			height="230"
			align="center"
			today_year="2026"
			today_month="5"
			today_day="15"
			shown_year="2026"
			shown_month="5"
		>
			<lv_calendar-header_arrow />
		</lv_calendar>
	</view>
</screen>
```
