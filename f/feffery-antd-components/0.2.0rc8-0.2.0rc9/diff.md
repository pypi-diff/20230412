# Comparing `tmp/feffery_antd_components-0.2.0rc8.tar.gz` & `tmp/feffery_antd_components-0.2.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_antd_components-0.2.0rc8.tar", last modified: Sun Oct  9 13:50:01 2022, max compression
+gzip compressed data, was "feffery_antd_components-0.2.0rc9.tar", last modified: Wed Oct 12 13:46:10 2022, max compression
```

## Comparing `feffery_antd_components-0.2.0rc8.tar` & `feffery_antd_components-0.2.0rc9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxrwx   0        0        0        0 2022-10-09 13:50:01.594773 feffery_antd_components-0.2.0rc8/
--rw-rw-rw-   0        0        0     1087 2022-10-09 09:26:38.000000 feffery_antd_components-0.2.0rc8/LICENSE
--rw-rw-rw-   0        0        0      288 2022-10-09 09:26:38.000000 feffery_antd_components-0.2.0rc8/MANIFEST.in
--rw-rw-rw-   0        0        0      381 2022-10-09 13:50:01.592776 feffery_antd_components-0.2.0rc8/PKG-INFO
--rw-rw-rw-   0        0        0     2150 2022-10-09 09:26:38.000000 feffery_antd_components-0.2.0rc8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-09 13:50:01.577816 feffery_antd_components-0.2.0rc8/feffery_antd_components/
--rw-rw-rw-   0        0        0     2586 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAccordion.py
--rw-rw-rw-   0        0        0     2332 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAccordionItem.py
--rw-rw-rw-   0        0        0     1998 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAffix.py
--rw-rw-rw-   0        0        0     2531 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAlert.py
--rw-rw-rw-   0        0        0     2212 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAnchor.py
--rw-rw-rw-   0        0        0     2568 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAvatar.py
--rw-rw-rw-   0        0        0     1885 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdBackTop.py
--rw-rw-rw-   0        0        0     2702 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdBadge.py
--rw-rw-rw-   0        0        0     2229 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdBreadcrumb.py
--rw-rw-rw-   0        0        0     3208 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdButton.py
--rw-rw-rw-   0        0        0     3349 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCalendar.py
--rw-rw-rw-   0        0        0     2862 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCard.py
--rw-rw-rw-   0        0        0     1913 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCardGrid.py
--rw-rw-rw-   0        0        0     2162 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCarousel.py
--rw-rw-rw-   0        0        0     5144 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCascader.py
--rw-rw-rw-   0        0        0     2298 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCheckCard.py
--rw-rw-rw-   0        0        0     2349 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCheckCardGroup.py
--rw-rw-rw-   0        0        0     3107 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCheckbox.py
--rw-rw-rw-   0        0        0     3291 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCheckboxGroup.py
--rw-rw-rw-   0        0        0     3886 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCol.py
--rw-rw-rw-   0        0        0     3672 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCollapse.py
--rw-rw-rw-   0        0        0     3896 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdComment.py
--rw-rw-rw-   0        0        0     1824 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdContent.py
--rw-rw-rw-   0        0        0     2102 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCopyText.py
--rw-rw-rw-   0        0        0     2441 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCountdown.py
--rw-rw-rw-   0        0        0     2530 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCustomSkeleton.py
--rw-rw-rw-   0        0        0     4961 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDatePicker.py
--rw-rw-rw-   0        0        0     4989 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDateRangePicker.py
--rw-rw-rw-   0        0        0     2189 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDescriptionItem.py
--rw-rw-rw-   0        0        0     2654 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDescriptions.py
--rw-rw-rw-   0        0        0     2569 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDivider.py
--rw-rw-rw-   0        0        0     4603 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDraggerUpload.py
--rw-rw-rw-   0        0        0     3006 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDrawer.py
--rw-rw-rw-   0        0        0     3241 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDropdown.py
--rw-rw-rw-   0        0        0     2224 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdEmpty.py
--rw-rw-rw-   0        0        0     1820 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdFooter.py
--rw-rw-rw-   0        0        0     2522 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdForm.py
--rw-rw-rw-   0        0        0     3051 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdFormItem.py
--rw-rw-rw-   0        0        0     1820 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdHeader.py
--rw-rw-rw-   0        0        0     1827 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdIcon.py
--rw-rw-rw-   0        0        0     5558 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdImage.py
--rw-rw-rw-   0        0        0     5619 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdInput.py
--rw-rw-rw-   0        0        0     4972 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdInputNumber.py
--rw-rw-rw-   0        0        0     1820 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdLayout.py
--rw-rw-rw-   0        0        0     2829 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdMentions.py
--rw-rw-rw-   0        0        0     3931 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdMenu.py
--rw-rw-rw-   0        0        0     2021 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdMessage.py
--rw-rw-rw-   0        0        0     4099 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdModal.py
--rw-rw-rw-   0        0        0     2400 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdNotification.py
--rw-rw-rw-   0        0        0     2548 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPageHeader.py
--rw-rw-rw-   0        0        0     4455 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPagination.py
--rw-rw-rw-   0        0        0     2752 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdParagraph.py
--rw-rw-rw-   0        0        0     2002 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPasteImage.py
--rw-rw-rw-   0        0        0     4448 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPictureUpload.py
--rw-rw-rw-   0        0        0     3795 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPopconfirm.py
--rw-rw-rw-   0        0        0     3328 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPopover.py
--rw-rw-rw-   0        0        0     3023 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPopupCard.py
--rw-rw-rw-   0        0        0     3240 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdProgress.py
--rw-rw-rw-   0        0        0     3903 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdRadioGroup.py
--rw-rw-rw-   0        0        0     2186 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdRate.py
--rw-rw-rw-   0        0        0     2168 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdResult.py
--rw-rw-rw-   0        0        0     2056 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdRibbon.py
--rw-rw-rw-   0        0        0     2472 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdRow.py
--rw-rw-rw-   0        0        0     3690 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSegmented.py
--rw-rw-rw-   0        0        0     3598 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSegmentedColoring.py
--rw-rw-rw-   0        0        0     6578 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSelect.py
--rw-rw-rw-   0        0        0     2820 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSider.py
--rw-rw-rw-   0        0        0     3170 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSkeleton.py
--rw-rw-rw-   0        0        0     1674 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSkeletonAvatar.py
--rw-rw-rw-   0        0        0     1751 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSkeletonButton.py
--rw-rw-rw-   0        0        0     1366 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSkeletonImage.py
--rw-rw-rw-   0        0        0     1556 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSkeletonInput.py
--rw-rw-rw-   0        0        0     2803 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSlider.py
--rw-rw-rw-   0        0        0     2377 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSpace.py
--rw-rw-rw-   0        0        0     2856 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSpin.py
--rw-rw-rw-   0        0        0     2584 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdStatistic.py
--rw-rw-rw-   0        0        0     2731 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSteps.py
--rw-rw-rw-   0        0        0     3447 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSwitch.py
--rw-rw-rw-   0        0        0     2321 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTabPane.py
--rw-rw-rw-   0        0        0    13380 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTable.py
--rw-rw-rw-   0        0        0     5110 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTabs.py
--rw-rw-rw-   0        0        0     1882 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTag.py
--rw-rw-rw-   0        0        0     2820 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdText.py
--rw-rw-rw-   0        0        0     4451 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTimePicker.py
--rw-rw-rw-   0        0        0     4507 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTimeRangePicker.py
--rw-rw-rw-   0        0        0     2802 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTimeline.py
--rw-rw-rw-   0        0        0     2899 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTitle.py
--rw-rw-rw-   0        0        0     3039 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTooltip.py
--rw-rw-rw-   0        0        0     4228 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTransfer.py
--rw-rw-rw-   0        0        0     4983 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTree.py
--rw-rw-rw-   0        0        0     5954 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTreeSelect.py
--rw-rw-rw-   0        0        0     4306 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdUpload.py
--rw-rw-rw-   0        0        0     2386 2022-10-09 13:42:52.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdWatermark.py
--rw-rw-rw-   0        0        0     1571 2022-10-09 09:26:38.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/__init__.py
--rw-rw-rw-   0        0        0     5688 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/_imports_.py
--rw-rw-rw-   0        0        0  3923444 2022-10-09 13:42:47.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/feffery_antd_components.min.js
--rw-rw-rw-   0        0        0   519979 2022-10-09 13:42:53.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/metadata.json
--rw-rw-rw-   0        0        0     2915 2022-10-09 13:42:49.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components/package-info.json
-drwxrwxrwx   0        0        0        0 2022-10-09 13:50:01.590781 feffery_antd_components-0.2.0rc8/feffery_antd_components.egg-info/
--rw-rw-rw-   0        0        0      381 2022-10-09 13:50:01.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4213 2022-10-09 13:50:01.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-09 13:50:01.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-10-09 13:50:01.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2022-10-09 13:50:01.000000 feffery_antd_components-0.2.0rc8/feffery_antd_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2915 2022-10-09 13:46:12.000000 feffery_antd_components-0.2.0rc8/package.json
--rw-rw-rw-   0        0        0       42 2022-10-09 13:50:01.595769 feffery_antd_components-0.2.0rc8/setup.cfg
--rw-rw-rw-   0        0        0      715 2022-10-09 09:26:38.000000 feffery_antd_components-0.2.0rc8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-12 13:46:10.444608 feffery_antd_components-0.2.0rc9/
+-rw-rw-rw-   0        0        0     1087 2022-10-09 09:26:38.000000 feffery_antd_components-0.2.0rc9/LICENSE
+-rw-rw-rw-   0        0        0      288 2022-10-09 09:26:38.000000 feffery_antd_components-0.2.0rc9/MANIFEST.in
+-rw-rw-rw-   0        0        0      381 2022-10-12 13:46:10.443611 feffery_antd_components-0.2.0rc9/PKG-INFO
+-rw-rw-rw-   0        0        0     2150 2022-10-09 09:26:38.000000 feffery_antd_components-0.2.0rc9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-12 13:46:10.432642 feffery_antd_components-0.2.0rc9/feffery_antd_components/
+-rw-rw-rw-   0        0        0     2586 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAccordion.py
+-rw-rw-rw-   0        0        0     2332 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAccordionItem.py
+-rw-rw-rw-   0        0        0     1998 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAffix.py
+-rw-rw-rw-   0        0        0     2531 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAlert.py
+-rw-rw-rw-   0        0        0     2212 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAnchor.py
+-rw-rw-rw-   0        0        0     2568 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAvatar.py
+-rw-rw-rw-   0        0        0     1885 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdBackTop.py
+-rw-rw-rw-   0        0        0     2702 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdBadge.py
+-rw-rw-rw-   0        0        0     2229 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdBreadcrumb.py
+-rw-rw-rw-   0        0        0     3208 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdButton.py
+-rw-rw-rw-   0        0        0     3349 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCalendar.py
+-rw-rw-rw-   0        0        0     2862 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCard.py
+-rw-rw-rw-   0        0        0     1913 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCardGrid.py
+-rw-rw-rw-   0        0        0     2162 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCarousel.py
+-rw-rw-rw-   0        0        0     5144 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCascader.py
+-rw-rw-rw-   0        0        0     2298 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCheckCard.py
+-rw-rw-rw-   0        0        0     2349 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCheckCardGroup.py
+-rw-rw-rw-   0        0        0     3107 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCheckbox.py
+-rw-rw-rw-   0        0        0     3291 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCheckboxGroup.py
+-rw-rw-rw-   0        0        0     3886 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCol.py
+-rw-rw-rw-   0        0        0     3672 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCollapse.py
+-rw-rw-rw-   0        0        0     3896 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdComment.py
+-rw-rw-rw-   0        0        0     1824 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdContent.py
+-rw-rw-rw-   0        0        0     2102 2022-10-12 13:45:22.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCopyText.py
+-rw-rw-rw-   0        0        0     2441 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCountdown.py
+-rw-rw-rw-   0        0        0     2530 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCustomSkeleton.py
+-rw-rw-rw-   0        0        0     4961 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDatePicker.py
+-rw-rw-rw-   0        0        0     4989 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDateRangePicker.py
+-rw-rw-rw-   0        0        0     2189 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDescriptionItem.py
+-rw-rw-rw-   0        0        0     2654 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDescriptions.py
+-rw-rw-rw-   0        0        0     2569 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDivider.py
+-rw-rw-rw-   0        0        0     4603 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDraggerUpload.py
+-rw-rw-rw-   0        0        0     3006 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDrawer.py
+-rw-rw-rw-   0        0        0     3241 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDropdown.py
+-rw-rw-rw-   0        0        0     2224 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdEmpty.py
+-rw-rw-rw-   0        0        0     1820 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdFooter.py
+-rw-rw-rw-   0        0        0     2522 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdForm.py
+-rw-rw-rw-   0        0        0     3051 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdFormItem.py
+-rw-rw-rw-   0        0        0     1820 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdHeader.py
+-rw-rw-rw-   0        0        0     1827 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdIcon.py
+-rw-rw-rw-   0        0        0     5558 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdImage.py
+-rw-rw-rw-   0        0        0     5619 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdInput.py
+-rw-rw-rw-   0        0        0     4972 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdInputNumber.py
+-rw-rw-rw-   0        0        0     1820 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdLayout.py
+-rw-rw-rw-   0        0        0     2829 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdMentions.py
+-rw-rw-rw-   0        0        0     3931 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdMenu.py
+-rw-rw-rw-   0        0        0     2021 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdMessage.py
+-rw-rw-rw-   0        0        0     4099 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdModal.py
+-rw-rw-rw-   0        0        0     2400 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdNotification.py
+-rw-rw-rw-   0        0        0     2548 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPageHeader.py
+-rw-rw-rw-   0        0        0     4455 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPagination.py
+-rw-rw-rw-   0        0        0     2752 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdParagraph.py
+-rw-rw-rw-   0        0        0     2002 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPasteImage.py
+-rw-rw-rw-   0        0        0     4448 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPictureUpload.py
+-rw-rw-rw-   0        0        0     3795 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPopconfirm.py
+-rw-rw-rw-   0        0        0     3328 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPopover.py
+-rw-rw-rw-   0        0        0     3023 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPopupCard.py
+-rw-rw-rw-   0        0        0     3240 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdProgress.py
+-rw-rw-rw-   0        0        0     3903 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdRadioGroup.py
+-rw-rw-rw-   0        0        0     2186 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdRate.py
+-rw-rw-rw-   0        0        0     2168 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdResult.py
+-rw-rw-rw-   0        0        0     2056 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdRibbon.py
+-rw-rw-rw-   0        0        0     2472 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdRow.py
+-rw-rw-rw-   0        0        0     3690 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSegmented.py
+-rw-rw-rw-   0        0        0     3598 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSegmentedColoring.py
+-rw-rw-rw-   0        0        0     6578 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSelect.py
+-rw-rw-rw-   0        0        0     2820 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSider.py
+-rw-rw-rw-   0        0        0     3170 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSkeleton.py
+-rw-rw-rw-   0        0        0     1674 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSkeletonAvatar.py
+-rw-rw-rw-   0        0        0     1751 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSkeletonButton.py
+-rw-rw-rw-   0        0        0     1366 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSkeletonImage.py
+-rw-rw-rw-   0        0        0     1556 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSkeletonInput.py
+-rw-rw-rw-   0        0        0     2803 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSlider.py
+-rw-rw-rw-   0        0        0     2377 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSpace.py
+-rw-rw-rw-   0        0        0     2856 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSpin.py
+-rw-rw-rw-   0        0        0     2584 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdStatistic.py
+-rw-rw-rw-   0        0        0     2731 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSteps.py
+-rw-rw-rw-   0        0        0     3447 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSwitch.py
+-rw-rw-rw-   0        0        0     2321 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTabPane.py
+-rw-rw-rw-   0        0        0    13370 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTable.py
+-rw-rw-rw-   0        0        0     5110 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTabs.py
+-rw-rw-rw-   0        0        0     1882 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTag.py
+-rw-rw-rw-   0        0        0     2820 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdText.py
+-rw-rw-rw-   0        0        0     4451 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTimePicker.py
+-rw-rw-rw-   0        0        0     4507 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTimeRangePicker.py
+-rw-rw-rw-   0        0        0     2802 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTimeline.py
+-rw-rw-rw-   0        0        0     2899 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTitle.py
+-rw-rw-rw-   0        0        0     3039 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTooltip.py
+-rw-rw-rw-   0        0        0     4228 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTransfer.py
+-rw-rw-rw-   0        0        0     4983 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTree.py
+-rw-rw-rw-   0        0        0     5954 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTreeSelect.py
+-rw-rw-rw-   0        0        0     4306 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdUpload.py
+-rw-rw-rw-   0        0        0     2386 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdWatermark.py
+-rw-rw-rw-   0        0        0     1571 2022-10-09 09:26:38.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/__init__.py
+-rw-rw-rw-   0        0        0     5688 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/_imports_.py
+-rw-rw-rw-   0        0        0  3923436 2022-10-12 13:45:18.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/feffery_antd_components.min.js
+-rw-rw-rw-   0        0        0   519417 2022-10-12 13:45:23.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/metadata.json
+-rw-rw-rw-   0        0        0     2915 2022-10-12 13:45:19.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components/package-info.json
+drwxrwxrwx   0        0        0        0 2022-10-12 13:46:10.441617 feffery_antd_components-0.2.0rc9/feffery_antd_components.egg-info/
+-rw-rw-rw-   0        0        0      381 2022-10-12 13:46:09.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4213 2022-10-12 13:46:10.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-12 13:46:09.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2022-10-12 13:46:09.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2022-10-12 13:46:09.000000 feffery_antd_components-0.2.0rc9/feffery_antd_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2915 2022-10-12 13:45:26.000000 feffery_antd_components-0.2.0rc9/package.json
+-rw-rw-rw-   0        0        0       42 2022-10-12 13:46:10.444608 feffery_antd_components-0.2.0rc9/setup.cfg
+-rw-rw-rw-   0        0        0      715 2022-10-09 09:26:38.000000 feffery_antd_components-0.2.0rc9/setup.py
```

### Comparing `feffery_antd_components-0.2.0rc8/LICENSE` & `feffery_antd_components-0.2.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/README.md` & `feffery_antd_components-0.2.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAccordion.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAccordion.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAccordionItem.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAccordionItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAffix.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAffix.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAlert.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAlert.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAnchor.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAnchor.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdAvatar.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdAvatar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdBackTop.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdBackTop.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdBadge.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdBadge.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdBreadcrumb.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdBreadcrumb.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdButton.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdButton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCalendar.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCalendar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCard.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCardGrid.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCardGrid.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCarousel.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCarousel.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCascader.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCascader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCheckCard.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCheckCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCheckCardGroup.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCheckCardGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCheckbox.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCheckbox.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCheckboxGroup.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCheckboxGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCol.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCol.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCollapse.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCollapse.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdComment.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdComment.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdContent.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdContent.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCopyText.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCopyText.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCountdown.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCountdown.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdCustomSkeleton.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdCustomSkeleton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDatePicker.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDatePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDateRangePicker.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDateRangePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDescriptionItem.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDescriptionItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDescriptions.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDescriptions.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDivider.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDivider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDraggerUpload.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDraggerUpload.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDrawer.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDrawer.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdDropdown.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdDropdown.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdEmpty.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdEmpty.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdFooter.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdFooter.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdForm.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdForm.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdFormItem.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdFormItem.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdHeader.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdHeader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdIcon.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdIcon.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdImage.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdInput.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdInput.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdInputNumber.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdInputNumber.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdLayout.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdLayout.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdMentions.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdMentions.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdMenu.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdMenu.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdMessage.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdMessage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdModal.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdModal.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdNotification.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdNotification.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPageHeader.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPageHeader.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPagination.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPagination.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdParagraph.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdParagraph.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPasteImage.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPasteImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPictureUpload.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPictureUpload.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPopconfirm.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPopconfirm.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPopover.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPopover.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdPopupCard.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdPopupCard.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdProgress.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdRadioGroup.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdRadioGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdRate.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdRate.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdResult.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdResult.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdRibbon.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdRibbon.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdRow.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdRow.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSegmented.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSegmented.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSegmentedColoring.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSegmentedColoring.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSelect.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSider.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSkeleton.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSkeleton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSkeletonAvatar.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSkeletonAvatar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSkeletonButton.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSkeletonButton.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSkeletonImage.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSkeletonImage.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSkeletonInput.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSkeletonInput.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSlider.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSlider.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSpace.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSpace.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSpin.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSpin.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdStatistic.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdStatistic.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSteps.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSteps.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdSwitch.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdSwitch.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTabPane.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTabPane.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTable.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTable.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
 - nClicksButton (number; default 0)
 
 - nClicksCell (number; default 0)
 
 - pagination (dict; optional)
 
-    `pagination` is a boolean | dict with keys:
+    `pagination` is a dict with keys:
 
     - current (number; optional)
 
     - disabled (boolean; optional)
 
     - hideOnSinglePage (boolean; optional)
```

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTabs.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTabs.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTag.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTag.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdText.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdText.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTimePicker.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTimePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTimeRangePicker.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTimeRangePicker.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTimeline.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTimeline.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTitle.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTitle.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTooltip.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTooltip.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTransfer.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTransfer.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTree.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTree.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdTreeSelect.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdTreeSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdUpload.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdUpload.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/AntdWatermark.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/AntdWatermark.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/__init__.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/_imports_.py` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/feffery_antd_components.min.js` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/feffery_antd_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,15 @@
     return Object.defineProperty(r, "p", {
         get: (t = o().src.split("/").slice(0, -1).join("/") + "/", function() {
             return t
         })
     }), "undefined" != typeof jsonpScriptSrc && (i = jsonpScriptSrc, jsonpScriptSrc = function(t) {
         var e, n = /\/_dash-component-suites\//.test(o().src),
             t = i(t);
-        return n ? ((e = (n = t.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-rc8m1665322925"), n.splice(-1, 1, e.join(".")), n.join("/")) : t
+        return n ? ((e = (n = t.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-rc9m1665582275"), n.splice(-1, 1, e.join(".")), n.join("/")) : t
     }), r(r.s = 752)
 }([function(t, e) {
     t.exports = window.React
 }, function(t, e) {
     t.exports = window.PropTypes
 }, function(R, t, e) {
     "use strict";
@@ -70631,17 +70631,18 @@
                         showTotalSuffix: null != (t = l.pagination) && t.showTotalSuffix ? null == (t = l.pagination) ? void 0 : t.showTotalSuffix : " 条记录"
                     })
                 }), c.state = {
                     searchText: "",
                     searchedColumn: ""
                 }, c.onPageChange = function(t, e, n, a) {
                     "paginate" === a.action ? l.setProps({
-                        pagination: _objectSpread(_objectSpread({}, t), {
-                            pageSize: null == t ? void 0 : t.pageSize,
-                            current: t.current
+                        pagination: _objectSpread(_objectSpread({}, t), {}, {
+                            pageSize: t.pageSize,
+                            current: t.current,
+                            position: t.position && Array.isArray(t.position) ? t.position[0] : t.position
                         }),
                         currentData: a.currentDataSource
                     }) : "sort" === a.action ? Array.isArray(n) ? l.setProps({
                         sorter: {
                             columns: n.map(function(t) {
                                 return t.column.dataIndex
                             }),
@@ -70899,15 +70900,15 @@
                         loading_state = _this$props.loading_state,
                         data = data || [],
                         size2size = new Map([
                             ["small", "default"],
                             ["default", "small"],
                             ["large", "middle"]
                         ]),
-                        i, pagination = _objectSpread(_objectSpread({}, pagination), {
+                        i, pagination = _objectSpread(_objectSpread({}, pagination), {}, {
                             showTotalPrefix: null != (_pagination = pagination) && _pagination.showTotalPrefix ? pagination.showTotalPrefix : "共 ",
                             showTotalSuffix: null != (_pagination2 = pagination) && _pagination2.showTotalSuffix ? pagination.showTotalSuffix : " 条记录"
                         }),
                         _i2;
                     for (i in data) data[i].hasOwnProperty("key") || (data[i].key = i.toString());
                     for (_i2 in columns) columns[_i2] = _objectSpread(_objectSpread({
                         align: "center"
@@ -71369,15 +71370,15 @@
                         rowSelection: rowSelection,
                         sticky: sticky,
                         pagination: _objectSpread(_objectSpread(_objectSpread({}, pagination), {
                             showTotal: function(t) {
                                 return "".concat(pagination.showTotalPrefix, " ").concat(t, " ").concat(pagination.showTotalSuffix)
                             }
                         }), {}, {
-                            position: pagination.position ? [pagination.position] : void 0
+                            position: pagination.position && !Array.isArray(pagination.position) ? [pagination.position] : pagination.position
                         }),
                         bordered: bordered,
                         scroll: {
                             x: maxWidth,
                             y: maxHeight,
                             scrollToFirstRowOnChange: !0
                         },
@@ -71526,15 +71527,15 @@
         }),
         filterOptions: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.objectOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.exact({
             filterMode: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOf(["checkbox", "keyword"]),
             filterCustomItems: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOfType([prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.arrayOf([prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string, prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number]), prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.any]),
             filterMultiple: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             filterSearch: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool
         })),
-        pagination: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOfType([prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool, prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.exact({
+        pagination: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.exact({
             position: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOf(["topLeft", "topCenter", "topRight", "bottomLeft", "bottomCenter", "bottomRight"]),
             pageSize: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
             current: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
             showSizeChanger: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             pageSizeOptions: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.arrayOf(prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number),
             showTitle: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             showQuickJumper: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
@@ -71542,15 +71543,15 @@
             showTotalSuffix: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.string,
             total: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
             hideOnSinglePage: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             simple: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             disabled: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             responsive: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
             size: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.oneOf(["default", "small"])
-        })]),
+        }),
         bordered: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.bool,
         maxHeight: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
         maxWidth: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
         currentData: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.array,
         recentlyChangedRow: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.object,
         recentlyButtonClickedRow: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.object,
         nClicksButton: prop_types__WEBPACK_IMPORTED_MODULE_1___default.a.number,
@@ -128638,15 +128639,15 @@
                     return g({
                         visible: !1
                     })
                 }
             }) : null),
             transitionName: "none" === u ? "" : "ant-".concat(u),
             width: s,
-            visible: l,
+            open: l,
             zIndex: h,
             bodyStyle: m,
             mask: !1,
             maskClosable: !1,
             closable: !1,
             footer: !1,
             wrapClassName: "ant-modal-wrap-overwrite",
```

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/metadata.json` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999499967998%*

 * *Differences: {"'src/lib/components/AntdTable.react.js'": "{'props': {'pagination': {'type': {'name': 'exact', "*

 * *                                            "'value': {replace: OrderedDict([('position', "*

 * *                                            "OrderedDict([('name', 'enum'), ('value', "*

 * *                                            '[OrderedDict([(\'value\', "\'topLeft\'"), '*

 * *                                            "('computed', False)]), OrderedDict([('value', "*

 * *                                            '"\'top […]*

```diff
@@ -12370,124 +12370,116 @@
                     "name": "number"
                 }
             },
             "pagination": {
                 "description": "",
                 "required": false,
                 "type": {
-                    "name": "union",
-                    "value": [
-                        {
-                            "name": "bool"
+                    "name": "exact",
+                    "value": {
+                        "current": {
+                            "name": "number",
+                            "required": false
                         },
-                        {
-                            "name": "exact",
+                        "disabled": {
+                            "name": "bool",
+                            "required": false
+                        },
+                        "hideOnSinglePage": {
+                            "name": "bool",
+                            "required": false
+                        },
+                        "pageSize": {
+                            "name": "number",
+                            "required": false
+                        },
+                        "pageSizeOptions": {
+                            "name": "arrayOf",
+                            "required": false,
                             "value": {
-                                "current": {
-                                    "name": "number",
-                                    "required": false
-                                },
-                                "disabled": {
-                                    "name": "bool",
-                                    "required": false
-                                },
-                                "hideOnSinglePage": {
-                                    "name": "bool",
-                                    "required": false
-                                },
-                                "pageSize": {
-                                    "name": "number",
-                                    "required": false
-                                },
-                                "pageSizeOptions": {
-                                    "name": "arrayOf",
-                                    "required": false,
-                                    "value": {
-                                        "name": "number"
-                                    }
-                                },
-                                "position": {
-                                    "name": "enum",
-                                    "required": false,
-                                    "value": [
-                                        {
-                                            "computed": false,
-                                            "value": "'topLeft'"
-                                        },
-                                        {
-                                            "computed": false,
-                                            "value": "'topCenter'"
-                                        },
-                                        {
-                                            "computed": false,
-                                            "value": "'topRight'"
-                                        },
-                                        {
-                                            "computed": false,
-                                            "value": "'bottomLeft'"
-                                        },
-                                        {
-                                            "computed": false,
-                                            "value": "'bottomCenter'"
-                                        },
-                                        {
-                                            "computed": false,
-                                            "value": "'bottomRight'"
-                                        }
-                                    ]
-                                },
-                                "responsive": {
-                                    "name": "bool",
-                                    "required": false
-                                },
-                                "showQuickJumper": {
-                                    "name": "bool",
-                                    "required": false
-                                },
-                                "showSizeChanger": {
-                                    "name": "bool",
-                                    "required": false
-                                },
-                                "showTitle": {
-                                    "name": "bool",
-                                    "required": false
-                                },
-                                "showTotalPrefix": {
-                                    "name": "string",
-                                    "required": false
-                                },
-                                "showTotalSuffix": {
-                                    "name": "string",
-                                    "required": false
-                                },
-                                "simple": {
-                                    "name": "bool",
-                                    "required": false
-                                },
-                                "size": {
-                                    "name": "enum",
-                                    "required": false,
-                                    "value": [
-                                        {
-                                            "computed": false,
-                                            "value": "'default'"
-                                        },
-                                        {
-                                            "computed": false,
-                                            "value": "'small'"
-                                        }
-                                    ]
-                                },
-                                "total": {
-                                    "name": "number",
-                                    "required": false
-                                }
+                                "name": "number"
                             }
+                        },
+                        "position": {
+                            "name": "enum",
+                            "required": false,
+                            "value": [
+                                {
+                                    "computed": false,
+                                    "value": "'topLeft'"
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "'topCenter'"
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "'topRight'"
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "'bottomLeft'"
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "'bottomCenter'"
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "'bottomRight'"
+                                }
+                            ]
+                        },
+                        "responsive": {
+                            "name": "bool",
+                            "required": false
+                        },
+                        "showQuickJumper": {
+                            "name": "bool",
+                            "required": false
+                        },
+                        "showSizeChanger": {
+                            "name": "bool",
+                            "required": false
+                        },
+                        "showTitle": {
+                            "name": "bool",
+                            "required": false
+                        },
+                        "showTotalPrefix": {
+                            "name": "string",
+                            "required": false
+                        },
+                        "showTotalSuffix": {
+                            "name": "string",
+                            "required": false
+                        },
+                        "simple": {
+                            "name": "bool",
+                            "required": false
+                        },
+                        "size": {
+                            "name": "enum",
+                            "required": false,
+                            "value": [
+                                {
+                                    "computed": false,
+                                    "value": "'default'"
+                                },
+                                {
+                                    "computed": false,
+                                    "value": "'small'"
+                                }
+                            ]
+                        },
+                        "total": {
+                            "name": "number",
+                            "required": false
                         }
-                    ]
+                    }
                 }
             },
             "recentlyButtonClickedRow": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "object"
```

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components/package-info.json` & `feffery_antd_components-0.2.0rc9/feffery_antd_components/package-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.0-rc9'"}*

```diff
@@ -81,9 +81,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_components -p package-info.json --r-prefix 'feffery' --jl-prefix 'feffery'",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-rc8"
+    "version": "0.2.0-rc9"
 }
```

### Comparing `feffery_antd_components-0.2.0rc8/feffery_antd_components.egg-info/SOURCES.txt` & `feffery_antd_components-0.2.0rc9/feffery_antd_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feffery_antd_components-0.2.0rc8/package.json` & `feffery_antd_components-0.2.0rc9/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.0-rc9'"}*

```diff
@@ -81,9 +81,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_components -p package-info.json --r-prefix 'feffery' --jl-prefix 'feffery'",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-rc8"
+    "version": "0.2.0-rc9"
 }
```

### Comparing `feffery_antd_components-0.2.0rc8/setup.py` & `feffery_antd_components-0.2.0rc9/setup.py`

 * *Files identical despite different names*

