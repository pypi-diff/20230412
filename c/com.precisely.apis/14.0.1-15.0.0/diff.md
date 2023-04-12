# Comparing `tmp/com.precisely.apis-14.0.1.tar.gz` & `tmp/com.precisely.apis-15.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.precisely.apis-14.0.1.tar", last modified: Thu Mar 16 09:16:39 2023, max compression
+gzip compressed data, was "com.precisely.apis-15.0.0.tar", last modified: Wed Apr 12 08:08:25 2023, max compression
```

## Comparing `com.precisely.apis-14.0.1.tar` & `com.precisely.apis-15.0.0.tar`

### file list

```diff
@@ -1,407 +1,409 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 09:16:39.358684 com.precisely.apis-14.0.1/
--rw-rw-rw-   0        0        0    11558 2023-02-22 08:43:21.000000 com.precisely.apis-14.0.1/LICENSE
--rw-rw-rw-   0        0        0      451 2023-03-16 09:16:39.359684 com.precisely.apis-14.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    48472 2023-03-16 09:11:59.000000 com.precisely.apis-14.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-16 09:16:38.652687 com.precisely.apis-14.0.1/com/
--rw-rw-rw-   0        0        0        0 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:16:38.681685 com.precisely.apis-14.0.1/com/precisely/
--rw-rw-rw-   0        0        0        0 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:16:38.695684 com.precisely.apis-14.0.1/com/precisely/apis/
--rw-rw-rw-   0        0        0      828 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:16:38.744684 com.precisely.apis-14.0.1/com/precisely/apis/api/
--rw-rw-rw-   0        0        0      241 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/__init__.py
--rw-rw-rw-   0        0        0    10596 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/address_autocomplete_service_api.py
--rw-rw-rw-   0        0        0    30342 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/address_verification_service_api.py
--rw-rw-rw-   0        0        0    23486 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/addresses_service__api.py
--rw-rw-rw-   0        0        0    43156 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/demographics_service_api.py
--rw-rw-rw-   0        0        0     5850 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/email_verification_service_api.py
--rw-rw-rw-   0        0        0    47771 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/geocode_service_api.py
--rw-rw-rw-   0        0        0    11824 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/geolocation_service_api.py
--rw-rw-rw-   0        0        0    53765 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/local_tax_service_api.py
--rw-rw-rw-   0        0        0     6043 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/neighborhoods_service__api.py
--rw-rw-rw-   0        0        0     6073 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/phone_verification_service_api.py
--rw-rw-rw-   0        0        0    66565 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/places_service__api.py
--rw-rw-rw-   0        0        0    11086 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/property_information_service_api.py
--rw-rw-rw-   0        0        0    20787 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/psap_911_service_api.py
--rw-rw-rw-   0        0        0   130591 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/risks_service_api.py
--rw-rw-rw-   0        0        0    57552 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/routing_service_api.py
--rw-rw-rw-   0        0        0    10365 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/schools_service_api.py
--rw-rw-rw-   0        0        0    19115 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/streets_service_api.py
--rw-rw-rw-   0        0        0    11525 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/telecomm_info_service_api.py
--rw-rw-rw-   0        0        0    21579 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/time_zone_service_api.py
--rw-rw-rw-   0        0        0    54012 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api/zones_service_api.py
--rw-rw-rw-   0        0        0    38556 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/api_client.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:16:38.747686 com.precisely.apis-14.0.1/com/precisely/apis/apis/
--rw-rw-rw-   0        0        0     2075 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/apis/__init__.py
--rw-rw-rw-   0        0        0    16559 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/configuration.py
--rw-rw-rw-   0        0        0     5117 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:16:39.354685 com.precisely.apis-14.0.1/com/precisely/apis/model/
--rw-rw-rw-   0        0        0      348 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/__init__.py
--rw-rw-rw-   0        0        0    11256 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/absentee_owner.py
--rw-rw-rw-   0        0        0    11241 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/accuracy.py
--rw-rw-rw-   0        0        0    17255 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/address.py
--rw-rw-rw-   0        0        0    11453 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/address_time.py
--rw-rw-rw-   0        0        0    11285 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/address_type.py
--rw-rw-rw-   0        0        0    13513 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/addresses_by_boundary_request.py
--rw-rw-rw-   0        0        0    11159 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/addresses_count.py
--rw-rw-rw-   0        0        0    14966 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/addresses_dto.py
--rw-rw-rw-   0        0        0    11321 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/addresses_preferences.py
--rw-rw-rw-   0        0        0    11720 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/addresses_response.py
--rw-rw-rw-   0        0        0    17285 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/ah_jmailing_address.py
--rw-rw-rw-   0        0        0    13338 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/ahj.py
--rw-rw-rw-   0        0        0    11201 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/ahj_list.py
--rw-rw-rw-   0        0        0    11761 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/ahj_plus_psap_response.py
--rw-rw-rw-   0        0        0    11244 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/amenities.py
--rw-rw-rw-   0        0        0    11229 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/area.py
--rw-rw-rw-   0        0        0    12644 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/area_code_info.py
--rw-rw-rw-   0        0        0    12082 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/assets_and_wealth_theme.py
--rw-rw-rw-   0        0        0    11271 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/base_flood_elevation.py
--rw-rw-rw-   0        0        0    11253 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/basement_type.py
--rw-rw-rw-   0        0        0    12377 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/basic_boundary.py
--rw-rw-rw-   0        0        0    11770 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/boundaries.py
--rw-rw-rw-   0        0        0    12162 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/boundary.py
--rw-rw-rw-   0        0        0    11763 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/boundary_buffer.py
--rw-rw-rw-   0        0        0    11298 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/boundary_point.py
--rw-rw-rw-   0        0        0    11294 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/buffer_relation.py
--rw-rw-rw-   0        0        0    11250 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_class.py
--rw-rw-rw-   0        0        0    11262 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_condition.py
--rw-rw-rw-   0        0        0    11595 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_features_sqft.py
--rw-rw-rw-   0        0        0    11564 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_improve_area.py
--rw-rw-rw-   0        0        0    11268 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_improve_type.py
--rw-rw-rw-   0        0        0    11256 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_quality.py
--rw-rw-rw-   0        0        0    11250 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_style.py
--rw-rw-rw-   0        0        0    11247 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_type.py
--rw-rw-rw-   0        0        0    11247 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_view.py
--rw-rw-rw-   0        0        0    11271 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/building_sqft_source.py
--rw-rw-rw-   0        0        0    11247 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/business_id.py
--rw-rw-rw-   0        0        0    11253 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/ca_exemptions.py
--rw-rw-rw-   0        0        0    13761 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/candidate.py
--rw-rw-rw-   0        0        0    13100 2023-02-22 08:52:42.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/candidate_range.py
--rw-rw-rw-   0        0        0    12226 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/candidate_range_unit.py
--rw-rw-rw-   0        0        0    11233 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/carrier.py
--rw-rw-rw-   0        0        0    11930 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/category.py
--rw-rw-rw-   0        0        0    12296 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/category_metadata.py
--rw-rw-rw-   0        0        0    11224 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/cbsa.py
--rw-rw-rw-   0        0        0    12050 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/census.py
--rw-rw-rw-   0        0        0    11277 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/center.py
--rw-rw-rw-   0        0        0    11259 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/city.py
--rw-rw-rw-   0        0        0    11893 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/common_geometry.py
--rw-rw-rw-   0        0        0    11420 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/community.py
--rw-rw-rw-   0        0        0    11297 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/consistency_code.py
--rw-rw-rw-   0        0        0    11253 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/construction.py
--rw-rw-rw-   0        0        0    12222 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/contact_details.py
--rw-rw-rw-   0        0        0    12861 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/contact_person.py
--rw-rw-rw-   0        0        0    11250 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/cooling_type.py
--rw-rw-rw-   0        0        0    11691 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/cost.py
--rw-rw-rw-   0        0        0    11230 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/county.py
--rw-rw-rw-   0        0        0    11464 2023-02-17 12:30:18.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/coverage.py
--rw-rw-rw-   0        0        0    11830 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/crime_boundary.py
--rw-rw-rw-   0        0        0    11750 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/crime_index_theme.py
--rw-rw-rw-   0        0        0    11834 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/crime_risk_by_address_batch_request.py
--rw-rw-rw-   0        0        0    11851 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/crime_risk_by_location_batch_request.py
--rw-rw-rw-   0        0        0    11331 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/crime_risk_preferences.py
--rw-rw-rw-   0        0        0    12263 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/crime_risk_response.py
--rw-rw-rw-   0        0        0    11372 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/crime_risk_response_list.py
--rw-rw-rw-   0        0        0    11530 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/crs.py
--rw-rw-rw-   0        0        0    12065 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/demographics.py
--rw-rw-rw-   0        0        0    11567 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/demographics_advanced_preferences.py
--rw-rw-rw-   0        0        0    12118 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/demographics_advanced_request.py
--rw-rw-rw-   0        0        0    11960 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/demographics_geometry.py
--rw-rw-rw-   0        0        0    11557 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/demographics_geometry_crc.py
--rw-rw-rw-   0        0        0    15660 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/demographics_themes_v2.py
--rw-rw-rw-   0        0        0    11232 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/depth.py
--rw-rw-rw-   0        0        0    12301 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/device_status_network.py
--rw-rw-rw-   0        0        0    11328 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/direction_geometry.py
--rw-rw-rw-   0        0        0    11241 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/distance.py
--rw-rw-rw-   0        0        0    11265 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/distance_to_border.py
--rw-rw-rw-   0        0        0    11863 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/distance_to_flood_hazard_address_request.py
--rw-rw-rw-   0        0        0    11880 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/distance_to_flood_hazard_location_request.py
--rw-rw-rw-   0        0        0    11406 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/distance_to_flood_hazard_response.py
--rw-rw-rw-   0        0        0    11288 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/district_type.py
--rw-rw-rw-   0        0        0    11635 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/domestic_ultimate_business.py
--rw-rw-rw-   0        0        0    11266 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_date_time.py
--rw-rw-rw-   0        0        0    13648 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_event.py
--rw-rw-rw-   0        0        0    11621 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_events_response.py
--rw-rw-rw-   0        0        0    11981 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_history.py
--rw-rw-rw-   0        0        0    11313 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_location.py
--rw-rw-rw-   0        0        0    11798 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11815 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_risk_by_location_request.py
--rw-rw-rw-   0        0        0    12371 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_risk_response.py
--rw-rw-rw-   0        0        0    11447 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_risk_response_list.py
--rw-rw-rw-   0        0        0    12064 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/education_theme.py
--rw-rw-rw-   0        0        0    11358 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/employee_count.py
--rw-rw-rw-   0        0        0    12067 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/employment_theme.py
--rw-rw-rw-   0        0        0    11247 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/energy_type.py
--rw-rw-rw-   0        0        0    11332 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/error_code.py
--rw-rw-rw-   0        0        0    11260 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/error_info.py
--rw-rw-rw-   0        0        0    13880 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/events_count.py
--rw-rw-rw-   0        0        0    12070 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/expenditure_theme.py
--rw-rw-rw-   0        0        0    11256 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/exterior_walls.py
--rw-rw-rw-   0        0        0    11589 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/extra_feature_sqft.py
--rw-rw-rw-   0        0        0    11445 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/field.py
--rw-rw-rw-   0        0        0    14301 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fields_matching.py
--rw-rw-rw-   0        0        0    12318 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_department.py
--rw-rw-rw-   0        0        0    12050 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_event.py
--rw-rw-rw-   0        0        0    11282 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_events_response.py
--rw-rw-rw-   0        0        0    11733 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_history.py
--rw-rw-rw-   0        0        0    11780 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11797 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_risk_by_location_request.py
--rw-rw-rw-   0        0        0    12122 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_risk_response.py
--rw-rw-rw-   0        0        0    11357 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_risk_response_list.py
--rw-rw-rw-   0        0        0    11725 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_shed.py
--rw-rw-rw-   0        0        0    13259 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_station.py
--rw-rw-rw-   0        0        0    11677 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_station_contact_details.py
--rw-rw-rw-   0        0        0    11677 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fire_stations.py
--rw-rw-rw-   0        0        0    11256 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fireplace_type.py
--rw-rw-rw-   0        0        0    11868 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/flood_hazard_preferences.py
--rw-rw-rw-   0        0        0    11819 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/flood_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11836 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/flood_risk_by_location_request.py
--rw-rw-rw-   0        0        0    11616 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/flood_risk_preferences.py
--rw-rw-rw-   0        0        0    12803 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/flood_risk_response.py
--rw-rw-rw-   0        0        0    11372 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/flood_risk_response_list.py
--rw-rw-rw-   0        0        0    12555 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/flood_zone.py
--rw-rw-rw-   0        0        0    11244 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/floor_type.py
--rw-rw-rw-   0        0        0    13506 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/formatted_tax_address.py
--rw-rw-rw-   0        0        0    11247 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/foundation.py
--rw-rw-rw-   0        0        0    11679 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/free_or_reduced_price_lunches.py
--rw-rw-rw-   0        0        0    11241 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/fuel_type.py
--rw-rw-rw-   0        0        0    11247 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/garage_type.py
--rw-rw-rw-   0        0        0    11682 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_access_point.py
--rw-rw-rw-   0        0        0    11479 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_country.py
--rw-rw-rw-   0        0        0    11298 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_fixed_line_country.py
--rw-rw-rw-   0        0        0    11957 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_ip_addr.py
--rw-rw-rw-   0        0        0    13204 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_place.py
--rw-rw-rw-   0        0        0    11295 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_state.py
--rw-rw-rw-   0        0        0    11638 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geo_pos.py
--rw-rw-rw-   0        0        0    14446 2023-02-22 08:52:02.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geocode_address.py
--rw-rw-rw-   0        0        0    18616 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geocode_preferences.py
--rw-rw-rw-   0        0        0    11970 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geocode_request.py
--rw-rw-rw-   0        0        0    12023 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geocode_service_response.py
--rw-rw-rw-   0        0        0    11418 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geocode_service_response_list.py
--rw-rw-rw-   0        0        0    11316 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geolocation_geometry.py
--rw-rw-rw-   0        0        0    11283 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geometry.py
--rw-rw-rw-   0        0        0    11521 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geometry_crc.py
--rw-rw-rw-   0        0        0    11088 2023-02-17 12:30:19.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/geometry_properties.py
--rw-rw-rw-   0        0        0    11461 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_input.py
--rw-rw-rw-   0        0        0    11984 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_input_row.py
--rw-rw-rw-   0        0        0    12600 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_options.py
--rw-rw-rw-   0        0        0    13593 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_output.py
--rw-rw-rw-   0        0        0    11912 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_request.py
--rw-rw-rw-   0        0        0    11470 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_response.py
--rw-rw-rw-   0        0        0    11400 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_input.py
--rw-rw-rw-   0        0        0    12159 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_input_row.py
--rw-rw-rw-   0        0        0    11710 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_options.py
--rw-rw-rw-   0        0        0    13110 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_output.py
--rw-rw-rw-   0        0        0    11316 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py
--rw-rw-rw-   0        0        0    11808 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_request.py
--rw-rw-rw-   0        0        0    11409 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_response.py
--rw-rw-rw-   0        0        0    11629 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/global_ultimate_business.py
--rw-rw-rw-   0        0        0    13489 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/grade_levels_taught.py
--rw-rw-rw-   0        0        0    11435 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/greatschools.py
--rw-rw-rw-   0        0        0    11462 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/grid.py
--rw-rw-rw-   0        0        0    12055 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/health_theme.py
--rw-rw-rw-   0        0        0    11250 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/heating_type.py
--rw-rw-rw-   0        0        0    12067 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/households_theme.py
--rw-rw-rw-   0        0        0    12058 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/housing_theme.py
--rw-rw-rw-   0        0        0    12055 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/income_theme.py
--rw-rw-rw-   0        0        0    11874 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/index_variable.py
--rw-rw-rw-   0        0        0    11677 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/individual_value_variable.py
--rw-rw-rw-   0        0        0    11253 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/interior_wall.py
--rw-rw-rw-   0        0        0    11319 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/intermediate_points.py
--rw-rw-rw-   0        0        0    12291 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/intersection.py
--rw-rw-rw-   0        0        0    11679 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/intersection_response.py
--rw-rw-rw-   0        0        0    12067 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/ip_info.py
--rw-rw-rw-   0        0        0    13054 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/ipd.py
--rw-rw-rw-   0        0        0    11890 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/ipd_tax_by_address_batch_request.py
--rw-rw-rw-   0        0        0    11871 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/ipd_tax_jurisdiction.py
--rw-rw-rw-   0        0        0    11808 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/key_lookup_request.py
--rw-rw-rw-   0        0        0    11446 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/keys.py
--rw-rw-rw-   0        0        0    11238 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/land_use.py
--rw-rw-rw-   0        0        0    12232 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/lat_long_fields.py
--rw-rw-rw-   0        0        0    12064 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/life_style_theme.py
--rw-rw-rw-   0        0        0    11238 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/loc_code.py
--rw-rw-rw-   0        0        0    11343 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/local_tax_geometry.py
--rw-rw-rw-   0        0        0    14407 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/local_tax_preferences.py
--rw-rw-rw-   0        0        0    11217 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/location.py
--rw-rw-rw-   0        0        0    12025 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/location_time.py
--rw-rw-rw-   0        0        0    12175 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/magnitude.py
--rw-rw-rw-   0        0        0    11972 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/match.py
--rw-rw-rw-   0        0        0    17276 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/matched_address.py
--rw-rw-rw-   0        0        0    12342 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/matrix.py
--rw-rw-rw-   0        0        0    11221 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/mcd.py
--rw-rw-rw-   0        0        0    11652 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/metadata_response.py
--rw-rw-rw-   0        0        0    11474 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/name.py
--rw-rw-rw-   0        0        0    11298 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/neighborhoods_response.py
--rw-rw-rw-   0        0        0    13019 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/network.py
--rw-rw-rw-   0        0        0    11496 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/organization_type.py
--rw-rw-rw-   0        0        0    11247 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/other_rooms.py
--rw-rw-rw-   0        0        0    11256 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/owner_vest_type.py
--rw-rw-rw-   0        0        0    11899 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/owners.py
--rw-rw-rw-   0        0        0    11605 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/parent_business.py
--rw-rw-rw-   0        0        0    11412 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/pb_key_address_request.py
--rw-rw-rw-   0        0        0    11468 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/pb_key_response.py
--rw-rw-rw-   0        0        0    11250 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/pb_key_response_list.py
--rw-rw-rw-   0        0        0    11646 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/pbkey.py
--rw-rw-rw-   0        0        0    11847 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/phone_verification.py
--rw-rw-rw-   0        0        0    11592 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/place.py
--rw-rw-rw-   0        0        0    12220 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/places_response.py
--rw-rw-rw-   0        0        0    20808 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poi.py
--rw-rw-rw-   0        0        0    12870 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary.py
--rw-rw-rw-   0        0        0    11840 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary_address_request.py
--rw-rw-rw-   0        0        0    11900 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary_location_request.py
--rw-rw-rw-   0        0        0    11825 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary_locations.py
--rw-rw-rw-   0        0        0    11548 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary_preferences.py
--rw-rw-rw-   0        0        0    11333 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary_response.py
--rw-rw-rw-   0        0        0    11800 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poi_classification.py
--rw-rw-rw-   0        0        0    11116 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poi_count.py
--rw-rw-rw-   0        0        0    12954 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poi_count_request.py
--rw-rw-rw-   0        0        0    13374 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/poiby_geometry_request.py
--rw-rw-rw-   0        0        0    11725 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/points.py
--rw-rw-rw-   0        0        0    11241 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/pool_type.py
--rw-rw-rw-   0        0        0    12067 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/population_theme.py
--rw-rw-rw-   0        0        0    11114 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/preferenc_time_zone.py
--rw-rw-rw-   0        0        0    11280 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/primary_zone.py
--rw-rw-rw-   0        0        0    11256 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/prior_sale_code.py
--rw-rw-rw-   0        0        0    11265 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/prop_site_influene.py
--rw-rw-rw-   0        0        0    11106 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/properties.py
--rw-rw-rw-   0        0        0    46206 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/property_attributes.py
--rw-rw-rw-   0        0        0    11349 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/property_geometry.py
--rw-rw-rw-   0        0        0    11918 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/property_info_address_request.py
--rw-rw-rw-   0        0        0    11133 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/property_info_preferences.py
--rw-rw-rw-   0        0        0    12002 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/property_info_response.py
--rw-rw-rw-   0        0        0    11457 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/property_info_responses.py
--rw-rw-rw-   0        0        0    11696 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/proxy.py
--rw-rw-rw-   0        0        0    13793 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/psap_response.py
--rw-rw-rw-   0        0        0    12085 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/race_and_ethnicity_theme.py
--rw-rw-rw-   0        0        0    12626 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/range_variable.py
--rw-rw-rw-   0        0        0    11664 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/rate.py
--rw-rw-rw-   0        0        0    13755 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/rate_center_response.py
--rw-rw-rw-   0        0        0    12337 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/return_fields_descriptor.py
--rw-rw-rw-   0        0        0    11723 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/reverse_geocode_request.py
--rw-rw-rw-   0        0        0    14978 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/risk.py
--rw-rw-rw-   0        0        0    17267 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/risk_address.py
--rw-rw-rw-   0        0        0    11337 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/risk_geometry.py
--rw-rw-rw-   0        0        0    11797 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/risk_locations.py
--rw-rw-rw-   0        0        0    11601 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/risk_preferences.py
--rw-rw-rw-   0        0        0    11316 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/risks_boundaries.py
--rw-rw-rw-   0        0        0    11368 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/risks_crime_theme.py
--rw-rw-rw-   0        0        0    11536 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/risks_geometry_crc.py
--rw-rw-rw-   0        0        0    13324 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/road.py
--rw-rw-rw-   0        0        0    11256 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/roof_cover_type.py
--rw-rw-rw-   0        0        0    11256 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/roof_frame_type.py
--rw-rw-rw-   0        0        0    11256 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/roof_shape_type.py
--rw-rw-rw-   0        0        0    12381 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/route_direction.py
--rw-rw-rw-   0        0        0    11304 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/route_geometry.py
--rw-rw-rw-   0        0        0    13382 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/route_response.py
--rw-rw-rw-   0        0        0    13904 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/sales_tax.py
--rw-rw-rw-   0        0        0    11569 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/sales_volume.py
--rw-rw-rw-   0        0        0    19109 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/school.py
--rw-rw-rw-   0        0        0    12879 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/school_district.py
--rw-rw-rw-   0        0        0    13410 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/school_profile.py
--rw-rw-rw-   0        0        0    12471 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/school_ranking.py
--rw-rw-rw-   0        0        0    11996 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/schools_near_by_response.py
--rw-rw-rw-   0        0        0    11761 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/segmentation.py
--rw-rw-rw-   0        0        0    11365 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/segmentation_themes.py
--rw-rw-rw-   0        0        0    11268 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/shore_line_distance.py
--rw-rw-rw-   0        0        0    12022 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/sic.py
--rw-rw-rw-   0        0        0    12330 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/sic_metadata.py
--rw-rw-rw-   0        0        0    12078 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/site_details.py
--rw-rw-rw-   0        0        0    13485 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/situs_address.py
--rw-rw-rw-   0        0        0    12476 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/special_purpose_district.py
--rw-rw-rw-   0        0        0    11579 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/special_purpose_district_tax.py
--rw-rw-rw-   0        0        0    13049 2023-02-17 12:30:20.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/speed_limit.py
--rw-rw-rw-   0        0        0    11298 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/start_end_point.py
--rw-rw-rw-   0        0        0    11227 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/state.py
--rw-rw-rw-   0        0        0    11265 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/status.py
--rw-rw-rw-   0        0        0    11273 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/stories.py
--rw-rw-rw-   0        0        0    12424 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/student_ethnicity.py
--rw-rw-rw-   0        0        0    12082 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/supply_and_demand_theme.py
--rw-rw-rw-   0        0        0    18388 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_address.py
--rw-rw-rw-   0        0        0    11824 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_address_request.py
--rw-rw-rw-   0        0        0    11239 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_county.py
--rw-rw-rw-   0        0        0    13607 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_district_response.py
--rw-rw-rw-   0        0        0    11446 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_district_response_list.py
--rw-rw-rw-   0        0        0    11247 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_doc_type.py
--rw-rw-rw-   0        0        0    11253 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_exemption.py
--rw-rw-rw-   0        0        0    11334 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_geometry.py
--rw-rw-rw-   0        0        0    12257 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_jurisdiction.py
--rw-rw-rw-   0        0        0    11798 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_location_request.py
--rw-rw-rw-   0        0        0    11787 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_locations.py
--rw-rw-rw-   0        0        0    12845 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_place.py
--rw-rw-rw-   0        0        0    18168 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_rate_address.py
--rw-rw-rw-   0        0        0    11919 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_rate_address_request.py
--rw-rw-rw-   0        0        0    11810 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_rate_location_request.py
--rw-rw-rw-   0        0        0    17504 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_rate_matched_address.py
--rw-rw-rw-   0        0        0    14126 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_rate_response.py
--rw-rw-rw-   0        0        0    11346 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_responses.py
--rw-rw-rw-   0        0        0    11268 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_sales_price_code.py
--rw-rw-rw-   0        0        0    11236 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/tax_state.py
--rw-rw-rw-   0        0        0    11229 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/time.py
--rw-rw-rw-   0        0        0    11731 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/timezone_address_request.py
--rw-rw-rw-   0        0        0    11349 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/timezone_geometry.py
--rw-rw-rw-   0        0        0    11357 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/timezone_location_request.py
--rw-rw-rw-   0        0        0    15245 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/timezone_response.py
--rw-rw-rw-   0        0        0    11352 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/timezone_response_list.py
--rw-rw-rw-   0        0        0    11354 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/travel_boundaries.py
--rw-rw-rw-   0        0        0    11234 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/travel_boundary.py
--rw-rw-rw-   0        0        0    11283 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/travel_cost_matrix_response.py
--rw-rw-rw-   0        0        0    11229 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/type.py
--rw-rw-rw-   0        0        0    13867 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/typeahead_location.py
--rw-rw-rw-   0        0        0    11353 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/typeahead_locations.py
--rw-rw-rw-   0        0        0    11505 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/typeahead_range.py
--rw-rw-rw-   0        0        0    11363 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/typeahead_unit.py
--rw-rw-rw-   0        0        0    11235 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/unit.py
--rw-rw-rw-   0        0        0    13898 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/use_tax.py
--rw-rw-rw-   0        0        0    11238 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/vacancy.py
--rw-rw-rw-   0        0        0    11817 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_email_address_api_request.py
--rw-rw-rw-   0        0        0    11447 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_email_address_api_response.py
--rw-rw-rw-   0        0        0    11429 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_email_address_input.py
--rw-rw-rw-   0        0        0    16658 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_email_address_input_row.py
--rw-rw-rw-   0        0        0    15324 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_email_address_output.py
--rw-rw-rw-   0        0        0    11449 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_input.py
--rw-rw-rw-   0        0        0    13503 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_input_row.py
--rw-rw-rw-   0        0        0    11357 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_options.py
--rw-rw-rw-   0        0        0    15940 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_output.py
--rw-rw-rw-   0        0        0    11520 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_input.py
--rw-rw-rw-   0        0        0    14342 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_input_row.py
--rw-rw-rw-   0        0        0    15105 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_options.py
--rw-rw-rw-   0        0        0    39660 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_output.py
--rw-rw-rw-   0        0        0    12012 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_request.py
--rw-rw-rw-   0        0        0    11529 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_response.py
--rw-rw-rw-   0        0        0    11480 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_input.py
--rw-rw-rw-   0        0        0    13512 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_input_row.py
--rw-rw-rw-   0        0        0    14100 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_options.py
--rw-rw-rw-   0        0        0    18611 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_output.py
--rw-rw-rw-   0        0        0    11944 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_request.py
--rw-rw-rw-   0        0        0    11489 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_response.py
--rw-rw-rw-   0        0        0    11891 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_request.py
--rw-rw-rw-   0        0        0    11458 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_response.py
--rw-rw-rw-   0        0        0    11530 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py
--rw-rw-rw-   0        0        0    14701 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py
--rw-rw-rw-   0        0        0    36257 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py
--rw-rw-rw-   0        0        0    49413 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py
--rw-rw-rw-   0        0        0    12029 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py
--rw-rw-rw-   0        0        0    11539 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py
--rw-rw-rw-   0        0        0    11760 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/water_body.py
--rw-rw-rw-   0        0        0    11870 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/water_body_response.py
--rw-rw-rw-   0        0        0    17270 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/zones_address.py
--rw-rw-rw-   0        0        0    11334 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/zones_boundary_geometry.py
--rw-rw-rw-   0        0        0    11574 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/zones_contact_details.py
--rw-rw-rw-   0        0        0    11340 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/zones_geometry.py
--rw-rw-rw-   0        0        0    11091 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/zones_parent_business.py
--rw-rw-rw-   0        0        0    14879 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/zones_poi.py
--rw-rw-rw-   0        0        0    11851 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/zones_poi_classification.py
--rw-rw-rw-   0        0        0    11863 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/zones_poi_geometry.py
--rw-rw-rw-   0        0        0    11791 2023-02-17 12:30:21.000000 com.precisely.apis-14.0.1/com/precisely/apis/model/zones_sic.py
--rw-rw-rw-   0        0        0    81943 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/model_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:16:39.356685 com.precisely.apis-14.0.1/com/precisely/apis/models/
--rw-rw-rw-   0        0        0    26531 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/models/__init__.py
--rw-rw-rw-   0        0        0    14245 2023-02-17 12:30:22.000000 com.precisely.apis-14.0.1/com/precisely/apis/rest.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:16:38.679686 com.precisely.apis-14.0.1/com.precisely.apis.egg-info/
--rw-rw-rw-   0        0        0      451 2023-03-16 09:16:38.000000 com.precisely.apis-14.0.1/com.precisely.apis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18396 2023-03-16 09:16:38.000000 com.precisely.apis-14.0.1/com.precisely.apis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 09:16:38.000000 com.precisely.apis-14.0.1/com.precisely.apis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-03-16 09:16:38.000000 com.precisely.apis-14.0.1/com.precisely.apis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-16 09:16:38.000000 com.precisely.apis-14.0.1/com.precisely.apis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       76 2023-03-16 09:16:39.365684 com.precisely.apis-14.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-03-16 09:10:46.000000 com.precisely.apis-14.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:08:25.558723 com.precisely.apis-15.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-12 07:09:56.000000 com.precisely.apis-15.0.0/LICENSE
+-rw-rw-rw-   0        0        0      451 2023-04-12 08:08:25.559723 com.precisely.apis-15.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    48680 2023-04-12 07:15:21.000000 com.precisely.apis-15.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 08:08:21.373168 com.precisely.apis-15.0.0/com/
+-rw-rw-rw-   0        0        0        0 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:08:21.397786 com.precisely.apis-15.0.0/com/precisely/
+-rw-rw-rw-   0        0        0        0 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:08:21.456784 com.precisely.apis-15.0.0/com/precisely/apis/
+-rw-rw-rw-   0        0        0      828 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:08:21.678546 com.precisely.apis-15.0.0/com/precisely/apis/api/
+-rw-rw-rw-   0        0        0      241 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/__init__.py
+-rw-rw-rw-   0        0        0    10596 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/address_autocomplete_service_api.py
+-rw-rw-rw-   0        0        0    30342 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/address_verification_service_api.py
+-rw-rw-rw-   0        0        0    23486 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/addresses_service__api.py
+-rw-rw-rw-   0        0        0    43156 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/demographics_service_api.py
+-rw-rw-rw-   0        0        0     5850 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/email_verification_service_api.py
+-rw-rw-rw-   0        0        0    47771 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/geocode_service_api.py
+-rw-rw-rw-   0        0        0    11824 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/geolocation_service_api.py
+-rw-rw-rw-   0        0        0    53765 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/local_tax_service_api.py
+-rw-rw-rw-   0        0        0     6043 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/neighborhoods_service__api.py
+-rw-rw-rw-   0        0        0     5902 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/phone_verification_service_api.py
+-rw-rw-rw-   0        0        0    66565 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/places_service__api.py
+-rw-rw-rw-   0        0        0    11086 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/property_information_service_api.py
+-rw-rw-rw-   0        0        0    20787 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/psap_911_service_api.py
+-rw-rw-rw-   0        0        0   130591 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/risks_service_api.py
+-rw-rw-rw-   0        0        0    57552 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/routing_service_api.py
+-rw-rw-rw-   0        0        0    10365 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/schools_service_api.py
+-rw-rw-rw-   0        0        0    19115 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/streets_service_api.py
+-rw-rw-rw-   0        0        0    11525 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/telecomm_info_service_api.py
+-rw-rw-rw-   0        0        0    21579 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/time_zone_service_api.py
+-rw-rw-rw-   0        0        0    54012 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api/zones_service_api.py
+-rw-rw-rw-   0        0        0    38556 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/api_client.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:08:21.686565 com.precisely.apis-15.0.0/com/precisely/apis/apis/
+-rw-rw-rw-   0        0        0     2075 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/apis/__init__.py
+-rw-rw-rw-   0        0        0    16559 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/configuration.py
+-rw-rw-rw-   0        0        0     5117 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:08:25.547724 com.precisely.apis-15.0.0/com/precisely/apis/model/
+-rw-rw-rw-   0        0        0      348 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/__init__.py
+-rw-rw-rw-   0        0        0    11256 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/absentee_owner.py
+-rw-rw-rw-   0        0        0    11241 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/accuracy.py
+-rw-rw-rw-   0        0        0    17255 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/address.py
+-rw-rw-rw-   0        0        0    11453 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/address_time.py
+-rw-rw-rw-   0        0        0    11285 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/address_type.py
+-rw-rw-rw-   0        0        0    13513 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/addresses_by_boundary_request.py
+-rw-rw-rw-   0        0        0    11159 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/addresses_count.py
+-rw-rw-rw-   0        0        0    14966 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/addresses_dto.py
+-rw-rw-rw-   0        0        0    11321 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/addresses_preferences.py
+-rw-rw-rw-   0        0        0    11720 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/addresses_response.py
+-rw-rw-rw-   0        0        0    17285 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/ah_jmailing_address.py
+-rw-rw-rw-   0        0        0    13338 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/ahj.py
+-rw-rw-rw-   0        0        0    11201 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/ahj_list.py
+-rw-rw-rw-   0        0        0    11761 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/ahj_plus_psap_response.py
+-rw-rw-rw-   0        0        0    11244 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/amenities.py
+-rw-rw-rw-   0        0        0    11229 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/area.py
+-rw-rw-rw-   0        0        0    12644 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/area_code_info.py
+-rw-rw-rw-   0        0        0    12082 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/assets_and_wealth_theme.py
+-rw-rw-rw-   0        0        0    11271 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/base_flood_elevation.py
+-rw-rw-rw-   0        0        0    11253 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/basement_type.py
+-rw-rw-rw-   0        0        0    12377 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/basic_boundary.py
+-rw-rw-rw-   0        0        0    11770 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/boundaries.py
+-rw-rw-rw-   0        0        0    12162 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/boundary.py
+-rw-rw-rw-   0        0        0    11763 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/boundary_buffer.py
+-rw-rw-rw-   0        0        0    11298 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/boundary_point.py
+-rw-rw-rw-   0        0        0    11294 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/buffer_relation.py
+-rw-rw-rw-   0        0        0    11250 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_class.py
+-rw-rw-rw-   0        0        0    11262 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_condition.py
+-rw-rw-rw-   0        0        0    11595 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_features_sqft.py
+-rw-rw-rw-   0        0        0    11564 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_improve_area.py
+-rw-rw-rw-   0        0        0    11268 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_improve_type.py
+-rw-rw-rw-   0        0        0    11256 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_quality.py
+-rw-rw-rw-   0        0        0    11250 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_style.py
+-rw-rw-rw-   0        0        0    11247 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_type.py
+-rw-rw-rw-   0        0        0    11247 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_view.py
+-rw-rw-rw-   0        0        0    11271 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/building_sqft_source.py
+-rw-rw-rw-   0        0        0    11247 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/business_id.py
+-rw-rw-rw-   0        0        0    11253 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/ca_exemptions.py
+-rw-rw-rw-   0        0        0    13761 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/candidate.py
+-rw-rw-rw-   0        0        0    13101 2023-04-12 08:03:18.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/candidate_range.py
+-rw-rw-rw-   0        0        0    12226 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/candidate_range_unit.py
+-rw-rw-rw-   0        0        0    11233 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/carrier.py
+-rw-rw-rw-   0        0        0    11930 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/category.py
+-rw-rw-rw-   0        0        0    12296 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/category_metadata.py
+-rw-rw-rw-   0        0        0    11224 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/cbsa.py
+-rw-rw-rw-   0        0        0    12050 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/census.py
+-rw-rw-rw-   0        0        0    11277 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/center.py
+-rw-rw-rw-   0        0        0    11259 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/city.py
+-rw-rw-rw-   0        0        0    11893 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/common_geometry.py
+-rw-rw-rw-   0        0        0    11420 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/community.py
+-rw-rw-rw-   0        0        0    11297 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/consistency_code.py
+-rw-rw-rw-   0        0        0    11253 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/construction.py
+-rw-rw-rw-   0        0        0    12222 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/contact_details.py
+-rw-rw-rw-   0        0        0    12861 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/contact_person.py
+-rw-rw-rw-   0        0        0    11250 2023-04-12 05:44:08.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/cooling_type.py
+-rw-rw-rw-   0        0        0    11691 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/cost.py
+-rw-rw-rw-   0        0        0    11230 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/county.py
+-rw-rw-rw-   0        0        0    11464 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/coverage.py
+-rw-rw-rw-   0        0        0    11830 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/crime_boundary.py
+-rw-rw-rw-   0        0        0    11750 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/crime_index_theme.py
+-rw-rw-rw-   0        0        0    11834 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/crime_risk_by_address_batch_request.py
+-rw-rw-rw-   0        0        0    11851 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/crime_risk_by_location_batch_request.py
+-rw-rw-rw-   0        0        0    11331 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/crime_risk_preferences.py
+-rw-rw-rw-   0        0        0    12263 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/crime_risk_response.py
+-rw-rw-rw-   0        0        0    11372 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/crime_risk_response_list.py
+-rw-rw-rw-   0        0        0    11530 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/crs.py
+-rw-rw-rw-   0        0        0    12065 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/demographics.py
+-rw-rw-rw-   0        0        0    11567 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/demographics_advanced_preferences.py
+-rw-rw-rw-   0        0        0    12118 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/demographics_advanced_request.py
+-rw-rw-rw-   0        0        0    11960 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/demographics_geometry.py
+-rw-rw-rw-   0        0        0    11557 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/demographics_geometry_crc.py
+-rw-rw-rw-   0        0        0    15660 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/demographics_themes_v2.py
+-rw-rw-rw-   0        0        0    11232 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/depth.py
+-rw-rw-rw-   0        0        0    11328 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/direction_geometry.py
+-rw-rw-rw-   0        0        0    11241 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/distance.py
+-rw-rw-rw-   0        0        0    11265 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/distance_to_border.py
+-rw-rw-rw-   0        0        0    11863 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/distance_to_flood_hazard_address_request.py
+-rw-rw-rw-   0        0        0    11880 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/distance_to_flood_hazard_location_request.py
+-rw-rw-rw-   0        0        0    11406 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/distance_to_flood_hazard_response.py
+-rw-rw-rw-   0        0        0    11288 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/district_type.py
+-rw-rw-rw-   0        0        0    11635 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/domestic_ultimate_business.py
+-rw-rw-rw-   0        0        0    11266 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_date_time.py
+-rw-rw-rw-   0        0        0    13648 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_event.py
+-rw-rw-rw-   0        0        0    11621 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_events_response.py
+-rw-rw-rw-   0        0        0    11981 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_history.py
+-rw-rw-rw-   0        0        0    11313 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_location.py
+-rw-rw-rw-   0        0        0    11798 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11815 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    12371 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_risk_response.py
+-rw-rw-rw-   0        0        0    11447 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_risk_response_list.py
+-rw-rw-rw-   0        0        0    12064 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/education_theme.py
+-rw-rw-rw-   0        0        0    11358 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/employee_count.py
+-rw-rw-rw-   0        0        0    12067 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/employment_theme.py
+-rw-rw-rw-   0        0        0    11247 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/energy_type.py
+-rw-rw-rw-   0        0        0    11332 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/error_code.py
+-rw-rw-rw-   0        0        0    11260 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/error_info.py
+-rw-rw-rw-   0        0        0    13880 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/events_count.py
+-rw-rw-rw-   0        0        0    12070 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/expenditure_theme.py
+-rw-rw-rw-   0        0        0    11256 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/exterior_walls.py
+-rw-rw-rw-   0        0        0    11589 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/extra_feature_sqft.py
+-rw-rw-rw-   0        0        0    11445 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/field.py
+-rw-rw-rw-   0        0        0    14301 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fields_matching.py
+-rw-rw-rw-   0        0        0    12318 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_department.py
+-rw-rw-rw-   0        0        0    12050 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_event.py
+-rw-rw-rw-   0        0        0    11282 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_events_response.py
+-rw-rw-rw-   0        0        0    11733 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_history.py
+-rw-rw-rw-   0        0        0    11780 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11797 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    12122 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_risk_response.py
+-rw-rw-rw-   0        0        0    11357 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_risk_response_list.py
+-rw-rw-rw-   0        0        0    11725 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_shed.py
+-rw-rw-rw-   0        0        0    13259 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_station.py
+-rw-rw-rw-   0        0        0    11677 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_station_contact_details.py
+-rw-rw-rw-   0        0        0    11677 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fire_stations.py
+-rw-rw-rw-   0        0        0    11256 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fireplace_type.py
+-rw-rw-rw-   0        0        0    11868 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/flood_hazard_preferences.py
+-rw-rw-rw-   0        0        0    11819 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/flood_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11836 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/flood_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    11616 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/flood_risk_preferences.py
+-rw-rw-rw-   0        0        0    12803 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/flood_risk_response.py
+-rw-rw-rw-   0        0        0    11372 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/flood_risk_response_list.py
+-rw-rw-rw-   0        0        0    12555 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/flood_zone.py
+-rw-rw-rw-   0        0        0    11244 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/floor_type.py
+-rw-rw-rw-   0        0        0    13506 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/formatted_tax_address.py
+-rw-rw-rw-   0        0        0    11247 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/foundation.py
+-rw-rw-rw-   0        0        0    11679 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/free_or_reduced_price_lunches.py
+-rw-rw-rw-   0        0        0    11241 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/fuel_type.py
+-rw-rw-rw-   0        0        0    11247 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/garage_type.py
+-rw-rw-rw-   0        0        0    11682 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geo_location_access_point.py
+-rw-rw-rw-   0        0        0    11479 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geo_location_country.py
+-rw-rw-rw-   0        0        0    11957 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geo_location_ip_addr.py
+-rw-rw-rw-   0        0        0    13204 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geo_location_place.py
+-rw-rw-rw-   0        0        0    11295 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geo_location_state.py
+-rw-rw-rw-   0        0        0    11638 2023-04-12 05:44:09.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geo_pos.py
+-rw-rw-rw-   0        0        0    14446 2023-04-12 08:03:50.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geocode_address.py
+-rw-rw-rw-   0        0        0    18616 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geocode_preferences.py
+-rw-rw-rw-   0        0        0    11970 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geocode_request.py
+-rw-rw-rw-   0        0        0    12023 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geocode_service_response.py
+-rw-rw-rw-   0        0        0    11418 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geocode_service_response_list.py
+-rw-rw-rw-   0        0        0    11316 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geolocation_geometry.py
+-rw-rw-rw-   0        0        0    11283 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geometry.py
+-rw-rw-rw-   0        0        0    11521 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geometry_crc.py
+-rw-rw-rw-   0        0        0    11088 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/geometry_properties.py
+-rw-rw-rw-   0        0        0    11461 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_input.py
+-rw-rw-rw-   0        0        0    11984 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_input_row.py
+-rw-rw-rw-   0        0        0    12600 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_options.py
+-rw-rw-rw-   0        0        0    13593 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_output.py
+-rw-rw-rw-   0        0        0    11912 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_request.py
+-rw-rw-rw-   0        0        0    11470 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_response.py
+-rw-rw-rw-   0        0        0    11400 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_input.py
+-rw-rw-rw-   0        0        0    12159 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_input_row.py
+-rw-rw-rw-   0        0        0    11710 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_options.py
+-rw-rw-rw-   0        0        0    13110 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_output.py
+-rw-rw-rw-   0        0        0    11316 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py
+-rw-rw-rw-   0        0        0    11808 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_request.py
+-rw-rw-rw-   0        0        0    11409 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_response.py
+-rw-rw-rw-   0        0        0    11629 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/global_ultimate_business.py
+-rw-rw-rw-   0        0        0    13489 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/grade_levels_taught.py
+-rw-rw-rw-   0        0        0    11435 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/greatschools.py
+-rw-rw-rw-   0        0        0    11462 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/grid.py
+-rw-rw-rw-   0        0        0    12055 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/health_theme.py
+-rw-rw-rw-   0        0        0    11250 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/heating_type.py
+-rw-rw-rw-   0        0        0    12067 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/households_theme.py
+-rw-rw-rw-   0        0        0    12058 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/housing_theme.py
+-rw-rw-rw-   0        0        0    12055 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/income_theme.py
+-rw-rw-rw-   0        0        0    11874 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/index_variable.py
+-rw-rw-rw-   0        0        0    11677 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/individual_value_variable.py
+-rw-rw-rw-   0        0        0    11253 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/interior_wall.py
+-rw-rw-rw-   0        0        0    11319 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/intermediate_points.py
+-rw-rw-rw-   0        0        0    12291 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/intersection.py
+-rw-rw-rw-   0        0        0    11679 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/intersection_response.py
+-rw-rw-rw-   0        0        0    12067 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/ip_info.py
+-rw-rw-rw-   0        0        0    13054 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/ipd.py
+-rw-rw-rw-   0        0        0    11890 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/ipd_tax_by_address_batch_request.py
+-rw-rw-rw-   0        0        0    11871 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/ipd_tax_jurisdiction.py
+-rw-rw-rw-   0        0        0    11808 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/key_lookup_request.py
+-rw-rw-rw-   0        0        0    11446 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/keys.py
+-rw-rw-rw-   0        0        0    11238 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/land_use.py
+-rw-rw-rw-   0        0        0    12232 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/lat_long_fields.py
+-rw-rw-rw-   0        0        0    12064 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/life_style_theme.py
+-rw-rw-rw-   0        0        0    11238 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/loc_code.py
+-rw-rw-rw-   0        0        0    11343 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/local_tax_geometry.py
+-rw-rw-rw-   0        0        0    14407 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/local_tax_preferences.py
+-rw-rw-rw-   0        0        0    11217 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/location.py
+-rw-rw-rw-   0        0        0    12025 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/location_time.py
+-rw-rw-rw-   0        0        0    12175 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/magnitude.py
+-rw-rw-rw-   0        0        0    11972 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/match.py
+-rw-rw-rw-   0        0        0    17276 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/matched_address.py
+-rw-rw-rw-   0        0        0    12342 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/matrix.py
+-rw-rw-rw-   0        0        0    11221 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/mcd.py
+-rw-rw-rw-   0        0        0    11652 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/metadata_response.py
+-rw-rw-rw-   0        0        0    11474 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/name.py
+-rw-rw-rw-   0        0        0    11298 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/neighborhoods_response.py
+-rw-rw-rw-   0        0        0    13019 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/network.py
+-rw-rw-rw-   0        0        0    11496 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/organization_type.py
+-rw-rw-rw-   0        0        0    11247 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/other_rooms.py
+-rw-rw-rw-   0        0        0    11256 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/owner_vest_type.py
+-rw-rw-rw-   0        0        0    11899 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/owners.py
+-rw-rw-rw-   0        0        0    11605 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/parent_business.py
+-rw-rw-rw-   0        0        0    11412 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/pb_key_address_request.py
+-rw-rw-rw-   0        0        0    11468 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/pb_key_response.py
+-rw-rw-rw-   0        0        0    11250 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/pb_key_response_list.py
+-rw-rw-rw-   0        0        0    11646 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/pbkey.py
+-rw-rw-rw-   0        0        0    11383 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/phone_verification.py
+-rw-rw-rw-   0        0        0    12826 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/phone_verification_output.py
+-rw-rw-rw-   0        0        0    11592 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/place.py
+-rw-rw-rw-   0        0        0    12220 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/places_response.py
+-rw-rw-rw-   0        0        0    20808 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poi.py
+-rw-rw-rw-   0        0        0    12870 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary.py
+-rw-rw-rw-   0        0        0    11840 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary_address_request.py
+-rw-rw-rw-   0        0        0    11900 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary_location_request.py
+-rw-rw-rw-   0        0        0    11825 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary_locations.py
+-rw-rw-rw-   0        0        0    11548 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary_preferences.py
+-rw-rw-rw-   0        0        0    11333 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary_response.py
+-rw-rw-rw-   0        0        0    11800 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poi_classification.py
+-rw-rw-rw-   0        0        0    11116 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poi_count.py
+-rw-rw-rw-   0        0        0    12954 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poi_count_request.py
+-rw-rw-rw-   0        0        0    13374 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/poiby_geometry_request.py
+-rw-rw-rw-   0        0        0    11725 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/points.py
+-rw-rw-rw-   0        0        0    11241 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/pool_type.py
+-rw-rw-rw-   0        0        0    12067 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/population_theme.py
+-rw-rw-rw-   0        0        0    11114 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/preferenc_time_zone.py
+-rw-rw-rw-   0        0        0    11280 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/primary_zone.py
+-rw-rw-rw-   0        0        0    11256 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/prior_sale_code.py
+-rw-rw-rw-   0        0        0    11265 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/prop_site_influene.py
+-rw-rw-rw-   0        0        0    11106 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/properties.py
+-rw-rw-rw-   0        0        0    46206 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/property_attributes.py
+-rw-rw-rw-   0        0        0    11349 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/property_geometry.py
+-rw-rw-rw-   0        0        0    11918 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/property_info_address_request.py
+-rw-rw-rw-   0        0        0    11133 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/property_info_preferences.py
+-rw-rw-rw-   0        0        0    12002 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/property_info_response.py
+-rw-rw-rw-   0        0        0    11457 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/property_info_responses.py
+-rw-rw-rw-   0        0        0    11696 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/proxy.py
+-rw-rw-rw-   0        0        0    13793 2023-04-12 05:44:10.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/psap_response.py
+-rw-rw-rw-   0        0        0    12085 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/race_and_ethnicity_theme.py
+-rw-rw-rw-   0        0        0    12626 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/range_variable.py
+-rw-rw-rw-   0        0        0    11664 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/rate.py
+-rw-rw-rw-   0        0        0    13755 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/rate_center_response.py
+-rw-rw-rw-   0        0        0    12337 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/return_fields_descriptor.py
+-rw-rw-rw-   0        0        0    11723 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/reverse_geocode_request.py
+-rw-rw-rw-   0        0        0    14978 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/risk.py
+-rw-rw-rw-   0        0        0    17267 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/risk_address.py
+-rw-rw-rw-   0        0        0    11337 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/risk_geometry.py
+-rw-rw-rw-   0        0        0    11797 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/risk_locations.py
+-rw-rw-rw-   0        0        0    11601 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/risk_preferences.py
+-rw-rw-rw-   0        0        0    11316 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/risks_boundaries.py
+-rw-rw-rw-   0        0        0    11368 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/risks_crime_theme.py
+-rw-rw-rw-   0        0        0    11536 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/risks_geometry_crc.py
+-rw-rw-rw-   0        0        0    13324 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/road.py
+-rw-rw-rw-   0        0        0    11256 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/roof_cover_type.py
+-rw-rw-rw-   0        0        0    11256 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/roof_frame_type.py
+-rw-rw-rw-   0        0        0    11256 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/roof_shape_type.py
+-rw-rw-rw-   0        0        0    12381 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/route_direction.py
+-rw-rw-rw-   0        0        0    11304 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/route_geometry.py
+-rw-rw-rw-   0        0        0    13382 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/route_response.py
+-rw-rw-rw-   0        0        0    13904 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/sales_tax.py
+-rw-rw-rw-   0        0        0    11569 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/sales_volume.py
+-rw-rw-rw-   0        0        0    19109 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/school.py
+-rw-rw-rw-   0        0        0    12879 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/school_district.py
+-rw-rw-rw-   0        0        0    13410 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/school_profile.py
+-rw-rw-rw-   0        0        0    12471 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/school_ranking.py
+-rw-rw-rw-   0        0        0    11996 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/schools_near_by_response.py
+-rw-rw-rw-   0        0        0    11761 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/segmentation.py
+-rw-rw-rw-   0        0        0    11365 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/segmentation_themes.py
+-rw-rw-rw-   0        0        0    11268 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/shore_line_distance.py
+-rw-rw-rw-   0        0        0    12022 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/sic.py
+-rw-rw-rw-   0        0        0    12330 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/sic_metadata.py
+-rw-rw-rw-   0        0        0    12078 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/site_details.py
+-rw-rw-rw-   0        0        0    13485 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/situs_address.py
+-rw-rw-rw-   0        0        0    12476 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/special_purpose_district.py
+-rw-rw-rw-   0        0        0    11579 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/special_purpose_district_tax.py
+-rw-rw-rw-   0        0        0    13049 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/speed_limit.py
+-rw-rw-rw-   0        0        0    11298 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/start_end_point.py
+-rw-rw-rw-   0        0        0    11227 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/state.py
+-rw-rw-rw-   0        0        0    11265 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/status.py
+-rw-rw-rw-   0        0        0    11273 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/stories.py
+-rw-rw-rw-   0        0        0    12424 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/student_ethnicity.py
+-rw-rw-rw-   0        0        0    12082 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/supply_and_demand_theme.py
+-rw-rw-rw-   0        0        0    18388 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_address.py
+-rw-rw-rw-   0        0        0    11824 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_address_request.py
+-rw-rw-rw-   0        0        0    11239 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_county.py
+-rw-rw-rw-   0        0        0    13607 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_district_response.py
+-rw-rw-rw-   0        0        0    11446 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_district_response_list.py
+-rw-rw-rw-   0        0        0    11247 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_doc_type.py
+-rw-rw-rw-   0        0        0    11253 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_exemption.py
+-rw-rw-rw-   0        0        0    11334 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_geometry.py
+-rw-rw-rw-   0        0        0    12257 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_jurisdiction.py
+-rw-rw-rw-   0        0        0    11798 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_location_request.py
+-rw-rw-rw-   0        0        0    11787 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_locations.py
+-rw-rw-rw-   0        0        0    12845 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_place.py
+-rw-rw-rw-   0        0        0    18168 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_rate_address.py
+-rw-rw-rw-   0        0        0    11919 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_rate_address_request.py
+-rw-rw-rw-   0        0        0    11810 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_rate_location_request.py
+-rw-rw-rw-   0        0        0    17504 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_rate_matched_address.py
+-rw-rw-rw-   0        0        0    14126 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_rate_response.py
+-rw-rw-rw-   0        0        0    11346 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_responses.py
+-rw-rw-rw-   0        0        0    11268 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_sales_price_code.py
+-rw-rw-rw-   0        0        0    11236 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/tax_state.py
+-rw-rw-rw-   0        0        0    11229 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/time.py
+-rw-rw-rw-   0        0        0    11731 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/timezone_address_request.py
+-rw-rw-rw-   0        0        0    11349 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/timezone_geometry.py
+-rw-rw-rw-   0        0        0    11357 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/timezone_location_request.py
+-rw-rw-rw-   0        0        0    15245 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/timezone_response.py
+-rw-rw-rw-   0        0        0    11352 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/timezone_response_list.py
+-rw-rw-rw-   0        0        0    11354 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/travel_boundaries.py
+-rw-rw-rw-   0        0        0    11234 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/travel_boundary.py
+-rw-rw-rw-   0        0        0    11283 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/travel_cost_matrix_response.py
+-rw-rw-rw-   0        0        0    11229 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/type.py
+-rw-rw-rw-   0        0        0    13867 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/typeahead_location.py
+-rw-rw-rw-   0        0        0    11353 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/typeahead_locations.py
+-rw-rw-rw-   0        0        0    11505 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/typeahead_range.py
+-rw-rw-rw-   0        0        0    11363 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/typeahead_unit.py
+-rw-rw-rw-   0        0        0    11235 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/unit.py
+-rw-rw-rw-   0        0        0    13898 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/use_tax.py
+-rw-rw-rw-   0        0        0    11238 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/vacancy.py
+-rw-rw-rw-   0        0        0    11817 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_email_address_api_request.py
+-rw-rw-rw-   0        0        0    11447 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_email_address_api_response.py
+-rw-rw-rw-   0        0        0    11429 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_email_address_input.py
+-rw-rw-rw-   0        0        0    16658 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_email_address_input_row.py
+-rw-rw-rw-   0        0        0    15324 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_email_address_output.py
+-rw-rw-rw-   0        0        0    11449 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_input.py
+-rw-rw-rw-   0        0        0    13503 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_input_row.py
+-rw-rw-rw-   0        0        0    11357 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_options.py
+-rw-rw-rw-   0        0        0    15940 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_output.py
+-rw-rw-rw-   0        0        0    11520 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_input.py
+-rw-rw-rw-   0        0        0    14342 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_input_row.py
+-rw-rw-rw-   0        0        0    15105 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_options.py
+-rw-rw-rw-   0        0        0    39660 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_output.py
+-rw-rw-rw-   0        0        0    12012 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_request.py
+-rw-rw-rw-   0        0        0    11529 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_response.py
+-rw-rw-rw-   0        0        0    11480 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_input.py
+-rw-rw-rw-   0        0        0    13512 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_input_row.py
+-rw-rw-rw-   0        0        0    14100 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_options.py
+-rw-rw-rw-   0        0        0    18611 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_output.py
+-rw-rw-rw-   0        0        0    11944 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_request.py
+-rw-rw-rw-   0        0        0    11489 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_response.py
+-rw-rw-rw-   0        0        0    11891 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_request.py
+-rw-rw-rw-   0        0        0    11458 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_response.py
+-rw-rw-rw-   0        0        0    11530 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py
+-rw-rw-rw-   0        0        0    14701 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py
+-rw-rw-rw-   0        0        0    36257 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py
+-rw-rw-rw-   0        0        0    49413 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py
+-rw-rw-rw-   0        0        0    12029 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py
+-rw-rw-rw-   0        0        0    11539 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py
+-rw-rw-rw-   0        0        0    11488 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_phone_number_api_request.py
+-rw-rw-rw-   0        0        0    11521 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_phone_number_api_request_input.py
+-rw-rw-rw-   0        0        0    11377 2023-04-12 05:44:11.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/validate_phone_number_api_request_input_row.py
+-rw-rw-rw-   0        0        0    11760 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/water_body.py
+-rw-rw-rw-   0        0        0    11870 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/water_body_response.py
+-rw-rw-rw-   0        0        0    17270 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/zones_address.py
+-rw-rw-rw-   0        0        0    11334 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/zones_boundary_geometry.py
+-rw-rw-rw-   0        0        0    11574 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/zones_contact_details.py
+-rw-rw-rw-   0        0        0    11340 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/zones_geometry.py
+-rw-rw-rw-   0        0        0    11091 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/zones_parent_business.py
+-rw-rw-rw-   0        0        0    14879 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/zones_poi.py
+-rw-rw-rw-   0        0        0    11851 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/zones_poi_classification.py
+-rw-rw-rw-   0        0        0    11863 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/zones_poi_geometry.py
+-rw-rw-rw-   0        0        0    11791 2023-04-12 05:44:12.000000 com.precisely.apis-15.0.0/com/precisely/apis/model/zones_sic.py
+-rw-rw-rw-   0        0        0    81943 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/model_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:08:25.557723 com.precisely.apis-15.0.0/com/precisely/apis/models/
+-rw-rw-rw-   0        0        0    26774 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/models/__init__.py
+-rw-rw-rw-   0        0        0    14245 2023-04-12 05:44:13.000000 com.precisely.apis-15.0.0/com/precisely/apis/rest.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:08:21.395787 com.precisely.apis-15.0.0/com.precisely.apis.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-04-12 08:08:21.000000 com.precisely.apis-15.0.0/com.precisely.apis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18542 2023-04-12 08:08:21.000000 com.precisely.apis-15.0.0/com.precisely.apis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 08:08:21.000000 com.precisely.apis-15.0.0/com.precisely.apis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-12 08:08:21.000000 com.precisely.apis-15.0.0/com.precisely.apis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-12 08:08:21.000000 com.precisely.apis-15.0.0/com.precisely.apis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       76 2023-04-12 08:08:25.560727 com.precisely.apis-15.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1168 2023-04-12 07:15:58.000000 com.precisely.apis-15.0.0/setup.py
```

### Comparing `com.precisely.apis-14.0.1/LICENSE` & `com.precisely.apis-15.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-14.0.1/README.md` & `com.precisely.apis-15.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,16 @@
 
 [Click here](https://docs.precisely.com/docs/sftw/precisely-apis/main/en-us/webhelp/apis/About%20Document/about_this_doc.html) for detailed Documentation on Precisely APIs 
 # PreciselyAPIsPythonSDK
 Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 14.0.1
-- Package version: 14.0.1
+- API version: 15.0.0
+- Package version: 15.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://support.precisely.com](https://support.precisely.com)
 
 ## Requirements.
 
@@ -194,15 +194,15 @@
 *LocalTaxServiceApi* | [**get_specific_tax_rate_by_address**](docs/LocalTaxServiceApi.md#get_specific_tax_rate_by_address) | **GET** /localtax/v1/taxrate/{taxRateTypeId}/byaddress | Get Taxrate By Address
 *LocalTaxServiceApi* | [**get_specific_tax_rate_by_location**](docs/LocalTaxServiceApi.md#get_specific_tax_rate_by_location) | **GET** /localtax/v1/taxrate/{taxRateTypeId}/bylocation | Get Taxrate By Location
 *NeighborhoodsServiceApi* | [**get_place_by_location**](docs/NeighborhoodsServiceApi.md#get_place_by_location) | **GET** /neighborhoods/v1/place/bylocation | Place By Location.
 *PSAP911ServiceApi* | [**get_ahj_plus_psapby_address**](docs/PSAP911ServiceApi.md#get_ahj_plus_psapby_address) | **GET** /911/v1/ahj-psap/byaddress | AHJ &amp; PSAP By Address.
 *PSAP911ServiceApi* | [**get_ahj_plus_psapby_location**](docs/PSAP911ServiceApi.md#get_ahj_plus_psapby_location) | **GET** /911/v1/ahj-psap/bylocation | AHJ &amp; PSAP By Location
 *PSAP911ServiceApi* | [**get_psapby_address**](docs/PSAP911ServiceApi.md#get_psapby_address) | **GET** /911/v1/psap/byaddress | PSAP By Address.
 *PSAP911ServiceApi* | [**get_psapby_location**](docs/PSAP911ServiceApi.md#get_psapby_location) | **GET** /911/v1/psap/bylocation | PSAP By Location.
-*PhoneVerificationServiceApi* | [**phone_verification**](docs/PhoneVerificationServiceApi.md#phone_verification) | **GET** /phoneverification/v1/phoneverification | Phone verification.
+*PhoneVerificationServiceApi* | [**validatephonenumber**](docs/PhoneVerificationServiceApi.md#validatephonenumber) | **POST** /phoneverification/v2/validatephonenumber/results.json | Phone verification.
 *PlacesServiceApi* | [**get_category_code_metadata**](docs/PlacesServiceApi.md#get_category_code_metadata) | **GET** /places/v1/metadata/category | Category Code Metadata.
 *PlacesServiceApi* | [**get_poiby_id**](docs/PlacesServiceApi.md#get_poiby_id) | **GET** /places/v1/poi/{id} | Points Of Interest Details By Id
 *PlacesServiceApi* | [**get_pois_by_address**](docs/PlacesServiceApi.md#get_pois_by_address) | **GET** /places/v1/poi/byaddress | Get POIs By Address.
 *PlacesServiceApi* | [**get_pois_by_area**](docs/PlacesServiceApi.md#get_pois_by_area) | **GET** /places/v1/poi/byarea | GET Points Of Interest By Area.
 *PlacesServiceApi* | [**get_pois_by_geometry**](docs/PlacesServiceApi.md#get_pois_by_geometry) | **POST** /places/v1/poi/byboundary | Points Of Interest By Boundary
 *PlacesServiceApi* | [**get_pois_by_location**](docs/PlacesServiceApi.md#get_pois_by_location) | **GET** /places/v1/poi/bylocation | Get POIs By Location.
 *PlacesServiceApi* | [**get_pois_count**](docs/PlacesServiceApi.md#get_pois_count) | **POST** /places/v1/poicount | Points Of Interest Count
@@ -285,15 +285,15 @@
  - [Boundary](docs/Boundary.md)
  - [BoundaryBuffer](docs/BoundaryBuffer.md)
  - [BoundaryPoint](docs/BoundaryPoint.md)
  - [BufferRelation](docs/BufferRelation.md)
  - [BuildgClass](docs/BuildgClass.md)
  - [BuildgCondition](docs/BuildgCondition.md)
  - [BuildgFeaturesSqft](docs/BuildgFeaturesSqft.md)
- - [BuildgImprovArea](docs/BuildgImprovArea.md)
+ - [BuildgImproveArea](docs/BuildgImproveArea.md)
  - [BuildgImproveType](docs/BuildgImproveType.md)
  - [BuildgQuality](docs/BuildgQuality.md)
  - [BuildgStyle](docs/BuildgStyle.md)
  - [BuildgType](docs/BuildgType.md)
  - [BuildgView](docs/BuildgView.md)
  - [BuildingSqftSource](docs/BuildingSqftSource.md)
  - [BusinessId](docs/BusinessId.md)
@@ -329,15 +329,14 @@
  - [Demographics](docs/Demographics.md)
  - [DemographicsAdvancedPreferences](docs/DemographicsAdvancedPreferences.md)
  - [DemographicsAdvancedRequest](docs/DemographicsAdvancedRequest.md)
  - [DemographicsGeometry](docs/DemographicsGeometry.md)
  - [DemographicsGeometryCRC](docs/DemographicsGeometryCRC.md)
  - [DemographicsThemesV2](docs/DemographicsThemesV2.md)
  - [Depth](docs/Depth.md)
- - [DeviceStatusNetwork](docs/DeviceStatusNetwork.md)
  - [DirectionGeometry](docs/DirectionGeometry.md)
  - [Distance](docs/Distance.md)
  - [DistanceToBorder](docs/DistanceToBorder.md)
  - [DistanceToFloodHazardAddressRequest](docs/DistanceToFloodHazardAddressRequest.md)
  - [DistanceToFloodHazardLocationRequest](docs/DistanceToFloodHazardLocationRequest.md)
  - [DistanceToFloodHazardResponse](docs/DistanceToFloodHazardResponse.md)
  - [DistrictType](docs/DistrictType.md)
@@ -387,15 +386,14 @@
  - [FormattedTaxAddress](docs/FormattedTaxAddress.md)
  - [Foundation](docs/Foundation.md)
  - [FreeOrReducedPriceLunches](docs/FreeOrReducedPriceLunches.md)
  - [FuelType](docs/FuelType.md)
  - [GarageType](docs/GarageType.md)
  - [GeoLocationAccessPoint](docs/GeoLocationAccessPoint.md)
  - [GeoLocationCountry](docs/GeoLocationCountry.md)
- - [GeoLocationFixedLineCountry](docs/GeoLocationFixedLineCountry.md)
  - [GeoLocationIpAddr](docs/GeoLocationIpAddr.md)
  - [GeoLocationPlace](docs/GeoLocationPlace.md)
  - [GeoLocationState](docs/GeoLocationState.md)
  - [GeoPos](docs/GeoPos.md)
  - [GeocodeAddress](docs/GeocodeAddress.md)
  - [GeocodePreferences](docs/GeocodePreferences.md)
  - [GeocodeRequest](docs/GeocodeRequest.md)
@@ -469,14 +467,15 @@
  - [POIBoundaryPreferences](docs/POIBoundaryPreferences.md)
  - [POIBoundaryResponse](docs/POIBoundaryResponse.md)
  - [POIByGeometryRequest](docs/POIByGeometryRequest.md)
  - [PSAPResponse](docs/PSAPResponse.md)
  - [ParentBusiness](docs/ParentBusiness.md)
  - [Pbkey](docs/Pbkey.md)
  - [PhoneVerification](docs/PhoneVerification.md)
+ - [PhoneVerificationOutput](docs/PhoneVerificationOutput.md)
  - [Place](docs/Place.md)
  - [PlacesResponse](docs/PlacesResponse.md)
  - [Poi](docs/Poi.md)
  - [PoiBoundary](docs/PoiBoundary.md)
  - [PoiClassification](docs/PoiClassification.md)
  - [PoiCount](docs/PoiCount.md)
  - [PoiCountRequest](docs/PoiCountRequest.md)
@@ -601,14 +600,17 @@
  - [ValidateMailingAddressResponse](docs/ValidateMailingAddressResponse.md)
  - [ValidateMailingAddressUSCANAPIInput](docs/ValidateMailingAddressUSCANAPIInput.md)
  - [ValidateMailingAddressUSCANAPIInputRow](docs/ValidateMailingAddressUSCANAPIInputRow.md)
  - [ValidateMailingAddressUSCANAPIOptions](docs/ValidateMailingAddressUSCANAPIOptions.md)
  - [ValidateMailingAddressUSCANAPIOutput](docs/ValidateMailingAddressUSCANAPIOutput.md)
  - [ValidateMailingAddressUSCANAPIRequest](docs/ValidateMailingAddressUSCANAPIRequest.md)
  - [ValidateMailingAddressUSCANAPIResponse](docs/ValidateMailingAddressUSCANAPIResponse.md)
+ - [ValidatePhoneNumberAPIRequest](docs/ValidatePhoneNumberAPIRequest.md)
+ - [ValidatePhoneNumberAPIRequestInput](docs/ValidatePhoneNumberAPIRequestInput.md)
+ - [ValidatePhoneNumberAPIRequestInputRow](docs/ValidatePhoneNumberAPIRequestInputRow.md)
  - [WaterBody](docs/WaterBody.md)
  - [WaterBodyResponse](docs/WaterBodyResponse.md)
  - [ZonesAddress](docs/ZonesAddress.md)
  - [ZonesBoundaryGeometry](docs/ZonesBoundaryGeometry.md)
  - [ZonesContactDetails](docs/ZonesContactDetails.md)
  - [ZonesGeometry](docs/ZonesGeometry.md)
  - [ZonesParentBusiness](docs/ZonesParentBusiness.md)
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/__init__.py` & `com.precisely.apis-15.0.0/com/precisely/apis/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # flake8: noqa
 
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "14.0.0"
+__version__ = "15.0.0"
 
 # import ApiClient
 from com.precisely.apis.api_client import ApiClient
 
 # import Configuration
 from com.precisely.apis.configuration import Configuration
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/address_autocomplete_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/address_autocomplete_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/address_verification_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/address_verification_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/addresses_service__api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/addresses_service__api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/demographics_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/demographics_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/email_verification_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/email_verification_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/geocode_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/geocode_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/geolocation_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/geolocation_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/local_tax_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/local_tax_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/neighborhoods_service__api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/neighborhoods_service__api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/phone_verification_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/phone_verification_service_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -19,104 +19,100 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from com.precisely.apis.model.error_info import ErrorInfo
 from com.precisely.apis.model.phone_verification import PhoneVerification
+from com.precisely.apis.model.validate_phone_number_api_request import ValidatePhoneNumberAPIRequest
 
 
 class PhoneVerificationServiceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.phone_verification_endpoint = _Endpoint(
+        self.validatephonenumber_endpoint = _Endpoint(
             settings={
                 'response_type': (PhoneVerification,),
                 'auth': [
                     'oAuth2Password'
                 ],
-                'endpoint_path': '/phoneverification/v1/phoneverification',
-                'operation_id': 'phone_verification',
-                'http_method': 'GET',
+                'endpoint_path': '/phoneverification/v2/validatephonenumber/results.json',
+                'operation_id': 'validatephonenumber',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'phone_number',
-                    'include_network_info',
+                    'validate_phone_number_api_request',
                 ],
                 'required': [
-                    'phone_number',
+                    'validate_phone_number_api_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'phone_number':
-                        (str,),
-                    'include_network_info':
-                        (str,),
+                    'validate_phone_number_api_request':
+                        (ValidatePhoneNumberAPIRequest,),
                 },
                 'attribute_map': {
-                    'phone_number': 'phoneNumber',
-                    'include_network_info': 'includeNetworkInfo',
                 },
                 'location_map': {
-                    'phone_number': 'query',
-                    'include_network_info': 'query',
+                    'validate_phone_number_api_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'application/xml'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
 
-    def phone_verification(
+    def validatephonenumber(
         self,
-        phone_number,
+        validate_phone_number_api_request,
         **kwargs
     ):
         """Phone verification.  # noqa: E501
 
-        This service accepts a phone number as input and returns details distinguishing landline and wireless numbers and also checks if a wireless number can be located.  # noqa: E501
+        This service accepts a phone number as input and returns details distinguishing landline and wireless numbers.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.phone_verification(phone_number, async_req=True)
+        >>> thread = api.validatephonenumber(validate_phone_number_api_request, async_req=True)
         >>> result = thread.get()
 
         Args:
-            phone_number (str): E.164 formatted phone number. Accepts digits only. Country Code (1) optional for USA & CAN.
+            validate_phone_number_api_request (ValidatePhoneNumberAPIRequest):
 
         Keyword Args:
-            include_network_info (str): Y or N (default is Y) – if it is N, then network/carrier details will not be added in the response.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -158,11 +154,11 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['phone_number'] = \
-            phone_number
-        return self.phone_verification_endpoint.call_with_http_info(**kwargs)
+        kwargs['validate_phone_number_api_request'] = \
+            validate_phone_number_api_request
+        return self.validatephonenumber_endpoint.call_with_http_info(**kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/places_service__api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/places_service__api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/property_information_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/property_information_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/psap_911_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/psap_911_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/risks_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/risks_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/routing_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/routing_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/schools_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/schools_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/streets_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/streets_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/telecomm_info_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/telecomm_info_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/time_zone_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/time_zone_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api/zones_service_api.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api/zones_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/api_client.py` & `com.precisely.apis-15.0.0/com/precisely/apis/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -80,15 +80,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/14.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/15.0.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/apis/__init__.py` & `com.precisely.apis-15.0.0/com/precisely/apis/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/configuration.py` & `com.precisely.apis-15.0.0/com/precisely/apis/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -383,16 +383,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 14.0.0\n"\
-               "SDK Package Version: 14.0.0".\
+               "Version of the API: 15.0.0\n"\
+               "SDK Package Version: 15.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/exceptions.py` & `com.precisely.apis-15.0.0/com/precisely/apis/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/absentee_owner.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/absentee_owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/accuracy.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class Accuracy(ModelNormal):
+class Time(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'unit': (str,),  # noqa: E501
             'value': (str,),  # noqa: E501
+            'unit': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'unit': 'unit',  # noqa: E501
         'value': 'value',  # noqa: E501
+        'unit': 'unit',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Accuracy - a model defined in OpenAPI
+        """Time - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            unit (str): [optional]  # noqa: E501
             value (str): [optional]  # noqa: E501
+            unit (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Accuracy - a model defined in OpenAPI
+        """Time - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,16 +215,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            unit (str): [optional]  # noqa: E501
             value (str): [optional]  # noqa: E501
+            unit (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/address_time.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/address_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/address_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/address_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/addresses_by_boundary_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/addresses_by_boundary_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/addresses_count.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/addresses_count.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/addresses_dto.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/addresses_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/addresses_preferences.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/addresses_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/addresses_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/addresses_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/ah_jmailing_address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/ah_jmailing_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/ahj.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/ahj.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/ahj_list.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/ahj_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/ahj_plus_psap_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/ahj_plus_psap_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/amenities.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/amenities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/area.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/area.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/area_code_info.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/area_code_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/assets_and_wealth_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/assets_and_wealth_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/base_flood_elevation.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/base_flood_elevation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/basement_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/basement_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/basic_boundary.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/basic_boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/boundaries.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/boundaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/boundary.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/boundary_buffer.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/boundary_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/boundary_point.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/boundary_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/buffer_relation.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/buffer_relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_class.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_condition.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_features_sqft.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_features_sqft.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_improve_area.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_improve_area.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_improve_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_improve_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_quality.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_style.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_style.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/buildg_view.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/buildg_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/building_sqft_source.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/building_sqft_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/business_id.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/business_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/ca_exemptions.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/ca_exemptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/candidate.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/candidate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/candidate_range.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/candidate_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -102,15 +102,15 @@
         return {
             'place_name': (str,),  # noqa: E501
             'low_house': (str,),  # noqa: E501
             'high_house': (str,),  # noqa: E501
             'side': (str,),  # noqa: E501
             'odd_even_indicator': (str,),  # noqa: E501
             'units': ([CandidateRangeUnit],),  # noqa: E501
-            'custom_fields': (dict,)  # noqa: E501
+            'custom_values': (dict,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/candidate_range_unit.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/candidate_range_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/carrier.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/carrier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/category.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/category_metadata.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/category_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/cbsa.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/cbsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/census.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/census.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/center.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/center.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/city.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/city.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/common_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/common_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/community.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/consistency_code.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/consistency_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/construction.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/construction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/contact_details.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/contact_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/contact_person.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/contact_person.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/cooling_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/cooling_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/cost.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/cost.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/county.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/county.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/coverage.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/crime_boundary.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/crime_boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/crime_index_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/crime_index_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/crime_risk_by_address_batch_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/crime_risk_by_address_batch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/crime_risk_by_location_batch_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/crime_risk_by_location_batch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/crime_risk_preferences.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/crime_risk_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/crime_risk_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/crime_risk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/crime_risk_response_list.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/crime_risk_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/crs.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/crs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/demographics.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/demographics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/demographics_advanced_preferences.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/demographics_advanced_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/demographics_advanced_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/demographics_advanced_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/demographics_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/demographics_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/demographics_geometry_crc.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/demographics_geometry_crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/demographics_themes_v2.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/demographics_themes_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/depth.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/depth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/device_status_network.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/individual_value_variable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from com.precisely.apis.model.geo_location_fixed_line_country import GeoLocationFixedLineCountry
-    globals()['GeoLocationFixedLineCountry'] = GeoLocationFixedLineCountry
 
-
-class DeviceStatusNetwork(ModelNormal):
+class IndividualValueVariable(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,60 +62,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'carrier': (str,),  # noqa: E501
-            'call_type': (str,),  # noqa: E501
-            'loc_accuracy_support': (str,),  # noqa: E501
-            'national_number': (str,),  # noqa: E501
-            'country': (GeoLocationFixedLineCountry,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'year': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'carrier': 'carrier',  # noqa: E501
-        'call_type': 'callType',  # noqa: E501
-        'loc_accuracy_support': 'locAccuracySupport',  # noqa: E501
-        'national_number': 'nationalNumber',  # noqa: E501
-        'country': 'country',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'year': 'year',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DeviceStatusNetwork - a model defined in OpenAPI
+        """IndividualValueVariable - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,19 +136,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            carrier (str): [optional]  # noqa: E501
-            call_type (str): [optional]  # noqa: E501
-            loc_accuracy_support (str): [optional]  # noqa: E501
-            national_number (str): [optional]  # noqa: E501
-            country (GeoLocationFixedLineCountry): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            description (str): [optional]  # noqa: E501
+            year (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -197,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DeviceStatusNetwork - a model defined in OpenAPI
+        """IndividualValueVariable - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,19 +221,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            carrier (str): [optional]  # noqa: E501
-            call_type (str): [optional]  # noqa: E501
-            loc_accuracy_support (str): [optional]  # noqa: E501
-            national_number (str): [optional]  # noqa: E501
-            country (GeoLocationFixedLineCountry): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            description (str): [optional]  # noqa: E501
+            year (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/direction_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/direction_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/distance.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/distance_to_border.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/distance_to_border.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/distance_to_flood_hazard_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/distance_to_flood_hazard_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/distance_to_flood_hazard_location_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/distance_to_flood_hazard_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/distance_to_flood_hazard_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/distance_to_flood_hazard_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/district_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/district_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/domestic_ultimate_business.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/domestic_ultimate_business.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_date_time.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_date_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_event.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_events_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_events_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_history.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_location.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_risk_by_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_risk_by_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_risk_by_location_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_risk_by_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_risk_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_risk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/earthquake_risk_response_list.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/earthquake_risk_response_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/education_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/education_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/employee_count.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/employee_count.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/employment_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/employment_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/energy_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/energy_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/error_code.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/error_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/error_info.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/error_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/events_count.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/events_count.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/expenditure_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/expenditure_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/exterior_walls.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/exterior_walls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/extra_feature_sqft.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/extra_feature_sqft.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/field.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fields_matching.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fields_matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_department.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_department.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_event.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_events_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_events_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_history.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_risk_by_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_risk_by_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_risk_by_location_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_risk_by_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_risk_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_risk_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_risk_response_list.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_risk_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_shed.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_shed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_station.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_station.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_station_contact_details.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_station_contact_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fire_stations.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fire_stations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fireplace_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fireplace_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/flood_hazard_preferences.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/flood_hazard_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/flood_risk_by_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/flood_risk_by_address_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/flood_risk_by_location_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/flood_risk_by_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/flood_risk_preferences.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/flood_risk_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/flood_risk_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/flood_risk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/flood_risk_response_list.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/flood_risk_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/flood_zone.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/flood_zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/floor_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/floor_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/formatted_tax_address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/formatted_tax_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/foundation.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/foundation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/free_or_reduced_price_lunches.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/free_or_reduced_price_lunches.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/fuel_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/fuel_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/garage_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/garage_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_access_point.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geo_location_access_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_country.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geo_location_country.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_fixed_line_country.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/loc_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class GeoLocationFixedLineCountry(ModelNormal):
+class LocCode(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GeoLocationFixedLineCountry - a model defined in OpenAPI
+        """LocCode - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GeoLocationFixedLineCountry - a model defined in OpenAPI
+        """LocCode - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_ip_addr.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geo_location_ip_addr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_place.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geo_location_place.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geo_location_state.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geo_location_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geo_pos.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geo_pos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geocode_address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geocode_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -92,15 +92,15 @@
             'post_code1': (str,),  # noqa: E501
             'post_code2': (str,),  # noqa: E501
             'country': (str,),  # noqa: E501
             'address_number': (str,),  # noqa: E501
             'street_name': (str,),  # noqa: E501
             'unit_type': (str,),  # noqa: E501
             'unit_value': (str,),  # noqa: E501
-            'custom_fields': (dict,)  # noqa: E501
+            'custom_values': (dict,), # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geocode_preferences.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geocode_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geocode_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geocode_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geocode_service_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geocode_service_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geocode_service_response_list.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geocode_service_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geolocation_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geolocation_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geometry_crc.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geometry_crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/geometry_properties.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/geometry_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_input.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_input_row.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_options.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_output.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_city_state_province_api_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_city_state_province_api_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_input.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_input_row.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_options.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_output.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/get_postal_codes_api_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/get_postal_codes_api_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/global_ultimate_business.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/global_ultimate_business.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/grade_levels_taught.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/grade_levels_taught.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/greatschools.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/greatschools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/grid.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/health_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/health_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/heating_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/heating_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/households_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/households_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/housing_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/housing_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/income_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/income_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/index_variable.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/index_variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/individual_value_variable.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/pool_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class IndividualValueVariable(ModelNormal):
+class PoolType(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,41 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
-            'year': (str,),  # noqa: E501
+            'code': (str,),  # noqa: E501
             'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'year': 'year',  # noqa: E501
+        'code': 'code',  # noqa: E501
         'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """IndividualValueVariable - a model defined in OpenAPI
+        """PoolType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,17 +132,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            description (str): [optional]  # noqa: E501
-            year (str): [optional]  # noqa: E501
+            code (str): [optional]  # noqa: E501
             value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -188,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """IndividualValueVariable - a model defined in OpenAPI
+        """PoolType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,17 +215,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            description (str): [optional]  # noqa: E501
-            year (str): [optional]  # noqa: E501
+            code (str): [optional]  # noqa: E501
             value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/interior_wall.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/interior_wall.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/intermediate_points.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/intermediate_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/intersection.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/intersection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/intersection_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/intersection_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/ip_info.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/ip_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/ipd.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/ipd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/ipd_tax_by_address_batch_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/ipd_tax_by_address_batch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/ipd_tax_jurisdiction.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/ipd_tax_jurisdiction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/key_lookup_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/key_lookup_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/keys.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/land_use.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/land_use.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/lat_long_fields.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/lat_long_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/life_style_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/life_style_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/loc_code.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_sales_price_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class LocCode(ModelNormal):
+class TaxSalesPriceCode(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """LocCode - a model defined in OpenAPI
+        """TaxSalesPriceCode - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """LocCode - a model defined in OpenAPI
+        """TaxSalesPriceCode - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/local_tax_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/local_tax_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/local_tax_preferences.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/local_tax_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/location.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/location_time.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/location_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/magnitude.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/magnitude.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/match.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/matched_address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/matched_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/matrix.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/mcd.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/mcd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/metadata_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/metadata_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/name.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/name.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/neighborhoods_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/neighborhoods_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/network.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/organization_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/organization_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/other_rooms.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/other_rooms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/owner_vest_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/owner_vest_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/owners.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/owners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/parent_business.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/parent_business.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/pb_key_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/pb_key_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/pb_key_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/pb_key_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/pb_key_response_list.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/pb_key_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/pbkey.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/pbkey.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/phone_verification.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/risk_preferences.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from com.precisely.apis.model.device_status_network import DeviceStatusNetwork
-    globals()['DeviceStatusNetwork'] = DeviceStatusNetwork
 
-
-class PhoneVerification(ModelNormal):
+class RiskPreferences(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,56 +62,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'phone_number': (str,),  # noqa: E501
-            'network': (DeviceStatusNetwork,),  # noqa: E501
-            'privacy_consent_required': (str,),  # noqa: E501
+            'include_geometry': (str,),  # noqa: E501
+            'include_zone_desc': (str,),  # noqa: E501
+            'richter_value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'phone_number': 'phoneNumber',  # noqa: E501
-        'network': 'network',  # noqa: E501
-        'privacy_consent_required': 'privacyConsentRequired',  # noqa: E501
+        'include_geometry': 'includeGeometry',  # noqa: E501
+        'include_zone_desc': 'includeZoneDesc',  # noqa: E501
+        'richter_value': 'richterValue',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PhoneVerification - a model defined in OpenAPI
+        """RiskPreferences - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +134,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phone_number (str): [optional]  # noqa: E501
-            network (DeviceStatusNetwork): [optional]  # noqa: E501
-            privacy_consent_required (str): [optional]  # noqa: E501
+            include_geometry (str): [optional]  # noqa: E501
+            include_zone_desc (str): [optional]  # noqa: E501
+            richter_value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PhoneVerification - a model defined in OpenAPI
+        """RiskPreferences - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,17 +218,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phone_number (str): [optional]  # noqa: E501
-            network (DeviceStatusNetwork): [optional]  # noqa: E501
-            privacy_consent_required (str): [optional]  # noqa: E501
+            include_geometry (str): [optional]  # noqa: E501
+            include_zone_desc (str): [optional]  # noqa: E501
+            richter_value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/place.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/place.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/places_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/places_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poi.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary_location_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary_locations.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary_preferences.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poi_boundary_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poi_boundary_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poi_classification.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poi_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poi_count.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poi_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poi_count_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poi_count_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/poiby_geometry_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/poiby_geometry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/points.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/pool_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class PoolType(ModelNormal):
+class Type(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PoolType - a model defined in OpenAPI
+        """Type - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PoolType - a model defined in OpenAPI
+        """Type - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/population_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/population_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/preferenc_time_zone.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/preferenc_time_zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/primary_zone.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/primary_zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/prior_sale_code.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/prior_sale_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/prop_site_influene.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/prop_site_influene.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/properties.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/property_attributes.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/property_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/property_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/property_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/property_info_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/property_info_address_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/property_info_preferences.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/property_info_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/property_info_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/property_info_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/property_info_responses.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/property_info_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/proxy.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/psap_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/psap_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/race_and_ethnicity_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/race_and_ethnicity_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/range_variable.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/range_variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/rate.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/rate_center_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/rate_center_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/return_fields_descriptor.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/return_fields_descriptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/reverse_geocode_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/reverse_geocode_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/risk.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/risk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/risk_address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/risk_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/risk_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/risk_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/risk_locations.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/risk_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/risk_preferences.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_county.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class RiskPreferences(ModelNormal):
+class TaxCounty(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,39 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'include_geometry': (str,),  # noqa: E501
-            'include_zone_desc': (str,),  # noqa: E501
-            'richter_value': (str,),  # noqa: E501
+            'code': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'include_geometry': 'includeGeometry',  # noqa: E501
-        'include_zone_desc': 'includeZoneDesc',  # noqa: E501
-        'richter_value': 'richterValue',  # noqa: E501
+        'code': 'code',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RiskPreferences - a model defined in OpenAPI
+        """TaxCounty - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,17 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            include_geometry (str): [optional]  # noqa: E501
-            include_zone_desc (str): [optional]  # noqa: E501
-            richter_value (str): [optional]  # noqa: E501
+            code (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RiskPreferences - a model defined in OpenAPI
+        """TaxCounty - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -218,17 +215,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            include_geometry (str): [optional]  # noqa: E501
-            include_zone_desc (str): [optional]  # noqa: E501
-            richter_value (str): [optional]  # noqa: E501
+            code (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/risks_boundaries.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/risks_boundaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/risks_crime_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/risks_crime_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/risks_geometry_crc.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/risks_geometry_crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/road.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/road.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/roof_cover_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/roof_cover_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/roof_frame_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/roof_frame_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/roof_shape_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/roof_shape_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/route_direction.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/route_direction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/route_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/route_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/route_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/route_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/sales_tax.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/sales_tax.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/sales_volume.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/sales_volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/school.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/school.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/school_district.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/school_district.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/school_profile.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/school_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/school_ranking.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/school_ranking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/schools_near_by_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/schools_near_by_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/segmentation.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/segmentation_themes.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/segmentation_themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/shore_line_distance.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/shore_line_distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/sic.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/sic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/sic_metadata.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/sic_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/site_details.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/site_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/situs_address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/situs_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/special_purpose_district.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/special_purpose_district.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/special_purpose_district_tax.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/special_purpose_district_tax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/speed_limit.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/speed_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/start_end_point.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/start_end_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/state.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/status.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/stories.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/stories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/student_ethnicity.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/student_ethnicity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/supply_and_demand_theme.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/supply_and_demand_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_county.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_doc_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class TaxCounty(ModelNormal):
+class TaxDocType(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,36 +78,36 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'code': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'code': 'code',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaxCounty - a model defined in OpenAPI
+        """TaxDocType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,15 +133,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             code (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaxCounty - a model defined in OpenAPI
+        """TaxDocType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             code (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_district_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_district_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_district_response_list.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_district_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_doc_type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_exemption.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class TaxDocType(ModelNormal):
+class TaxExemption(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaxDocType - a model defined in OpenAPI
+        """TaxExemption - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaxDocType - a model defined in OpenAPI
+        """TaxExemption - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_exemption.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class TaxExemption(ModelNormal):
+class TaxState(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,36 +78,36 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'code': (str,),  # noqa: E501
-            'value': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'code': 'code',  # noqa: E501
-        'value': 'value',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaxExemption - a model defined in OpenAPI
+        """TaxState - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,15 +133,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             code (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaxExemption - a model defined in OpenAPI
+        """TaxState - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             code (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_jurisdiction.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_jurisdiction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_location_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_locations.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_place.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_place.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_rate_address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_rate_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_rate_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_rate_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_rate_location_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_rate_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_rate_matched_address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_rate_matched_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_rate_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_rate_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_responses.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/tax_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_sales_price_code.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/vacancy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class TaxSalesPriceCode(ModelNormal):
+class Vacancy(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaxSalesPriceCode - a model defined in OpenAPI
+        """Vacancy - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaxSalesPriceCode - a model defined in OpenAPI
+        """Vacancy - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/tax_state.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/zones_parent_business.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class TaxState(ModelNormal):
+class ZonesParentBusiness(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,35 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'code': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'code': 'code',  # noqa: E501
         'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaxState - a model defined in OpenAPI
+        """ZonesParentBusiness - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,15 +130,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            code (str): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -182,15 +179,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaxState - a model defined in OpenAPI
+        """ZonesParentBusiness - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,15 +212,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            code (str): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/time.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class Time(ModelNormal):
+class Accuracy(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),  # noqa: E501
             'unit': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'value': 'value',  # noqa: E501
         'unit': 'unit',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Time - a model defined in OpenAPI
+        """Accuracy - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str): [optional]  # noqa: E501
             unit (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Time - a model defined in OpenAPI
+        """Accuracy - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,16 +215,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (str): [optional]  # noqa: E501
             unit (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/timezone_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/timezone_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/timezone_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/timezone_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/timezone_location_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/timezone_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/timezone_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/timezone_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/timezone_response_list.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/timezone_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/travel_boundaries.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/travel_boundaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/travel_boundary.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/travel_boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/travel_cost_matrix_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/travel_cost_matrix_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/type.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class Type(ModelNormal):
+class Unit(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'code': (str,),  # noqa: E501
-            'value': (str,),  # noqa: E501
+            'value': (float,),  # noqa: E501
+            'unit': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'code': 'code',  # noqa: E501
         'value': 'value',  # noqa: E501
+        'unit': 'unit',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Type - a model defined in OpenAPI
+        """Unit - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            code (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
+            value (float): [optional]  # noqa: E501
+            unit (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Type - a model defined in OpenAPI
+        """Unit - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,16 +215,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            code (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
+            value (float): [optional]  # noqa: E501
+            unit (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/typeahead_location.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/typeahead_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/typeahead_locations.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/typeahead_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/typeahead_range.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/typeahead_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/typeahead_unit.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/typeahead_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/unit.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/phone_verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from com.precisely.apis.model.phone_verification_output import PhoneVerificationOutput
+    globals()['PhoneVerificationOutput'] = PhoneVerificationOutput
 
-class Unit(ModelNormal):
+
+class PhoneVerification(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,52 +66,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'value': (float,),  # noqa: E501
-            'unit': (str,),  # noqa: E501
+            'output': ([PhoneVerificationOutput],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'value': 'value',  # noqa: E501
-        'unit': 'unit',  # noqa: E501
+        'output': 'Output',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Unit - a model defined in OpenAPI
+        """PhoneVerification - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (float): [optional]  # noqa: E501
-            unit (str): [optional]  # noqa: E501
+            output ([PhoneVerificationOutput]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Unit - a model defined in OpenAPI
+        """PhoneVerification - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,16 +218,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            value (float): [optional]  # noqa: E501
-            unit (str): [optional]  # noqa: E501
+            output ([PhoneVerificationOutput]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/use_tax.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/use_tax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/vacancy.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/zones_boundary_geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class Vacancy(ModelNormal):
+class ZonesBoundaryGeometry(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,37 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'code': (str,),  # noqa: E501
-            'value': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'coordinates': ([[[float]]],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'code': 'code',  # noqa: E501
-        'value': 'value',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'coordinates': 'coordinates',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Vacancy - a model defined in OpenAPI
+        """ZonesBoundaryGeometry - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            code (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            coordinates ([[[float]]]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Vacancy - a model defined in OpenAPI
+        """ZonesBoundaryGeometry - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,16 +215,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            code (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            coordinates ([[[float]]]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_email_address_api_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_email_address_api_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_email_address_api_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_email_address_api_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_email_address_input.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_email_address_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_email_address_input_row.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_email_address_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_email_address_output.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_email_address_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_input.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_input_row.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_input_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_options.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_output.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_input.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_input_row.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_options.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_output.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_premium_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_premium_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_input.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_input_row.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_options.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_output.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_pro_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_pro_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/water_body.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/water_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/water_body_response.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/water_body_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/zones_address.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/zones_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/zones_boundary_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/zones_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class ZonesBoundaryGeometry(ModelNormal):
+class ZonesGeometry(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,15 +78,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'type': (str,),  # noqa: E501
-            'coordinates': ([[[float]]],),  # noqa: E501
+            'coordinates': ([float],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -98,16 +98,19 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ZonesBoundaryGeometry - a model defined in OpenAPI
+    def _from_openapi_data(cls, type, *args, **kwargs):  # noqa: E501
+        """ZonesGeometry - a model defined in OpenAPI
+
+        Args:
+            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +135,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            coordinates ([[[float]]]): [optional]  # noqa: E501
+            coordinates ([float]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -161,14 +163,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -181,16 +184,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """ZonesBoundaryGeometry - a model defined in OpenAPI
+    def __init__(self, type, *args, **kwargs):  # noqa: E501
+        """ZonesGeometry - a model defined in OpenAPI
+
+        Args:
+            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,16 +221,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            coordinates ([[[float]]]): [optional]  # noqa: E501
+            coordinates ([float]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -242,14 +247,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/zones_contact_details.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/zones_contact_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/zones_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_phone_number_api_request_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from com.precisely.apis.model.validate_phone_number_api_request_input_row import ValidatePhoneNumberAPIRequestInputRow
+    globals()['ValidatePhoneNumberAPIRequestInputRow'] = ValidatePhoneNumberAPIRequestInputRow
 
-class ZonesGeometry(ModelNormal):
+
+class ValidatePhoneNumberAPIRequestInput(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,55 +66,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'coordinates': ([float],),  # noqa: E501
+            'row': ([ValidatePhoneNumberAPIRequestInputRow],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'coordinates': 'coordinates',  # noqa: E501
+        'row': 'Row',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, type, *args, **kwargs):  # noqa: E501
-        """ZonesGeometry - a model defined in OpenAPI
-
-        Args:
-            type (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ValidatePhoneNumberAPIRequestInput - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            coordinates ([float]): [optional]  # noqa: E501
+            row ([ValidatePhoneNumberAPIRequestInputRow]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -163,15 +164,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -184,19 +184,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, type, *args, **kwargs):  # noqa: E501
-        """ZonesGeometry - a model defined in OpenAPI
-
-        Args:
-            type (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ValidatePhoneNumberAPIRequestInput - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,15 +218,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            coordinates ([float]): [optional]  # noqa: E501
+            row ([ValidatePhoneNumberAPIRequestInputRow]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,15 +244,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/zones_parent_business.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/validate_phone_number_api_request_input_row.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class ZonesParentBusiness(ModelNormal):
+class ValidatePhoneNumberAPIRequestInputRow(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,35 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str,),  # noqa: E501
+            'phone_number': (str,),  # noqa: E501
+            'country': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
+        'phone_number': 'PhoneNumber',  # noqa: E501
+        'country': 'Country',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ZonesParentBusiness - a model defined in OpenAPI
+        """ValidatePhoneNumberAPIRequestInputRow - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            phone_number (str): [optional]  # noqa: E501
+            country (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -179,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ZonesParentBusiness - a model defined in OpenAPI
+        """ValidatePhoneNumberAPIRequestInputRow - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -212,15 +215,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            phone_number (str): [optional]  # noqa: E501
+            country (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/zones_poi.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/zones_poi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/zones_poi_classification.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/zones_poi_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/zones_poi_geometry.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/zones_poi_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model/zones_sic.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model/zones_sic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/model_utils.py` & `com.precisely.apis-15.0.0/com/precisely/apis/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/models/__init__.py` & `com.precisely.apis-15.0.0/com/precisely/apis/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 from com.precisely.apis.model.demographics import Demographics
 from com.precisely.apis.model.demographics_advanced_preferences import DemographicsAdvancedPreferences
 from com.precisely.apis.model.demographics_advanced_request import DemographicsAdvancedRequest
 from com.precisely.apis.model.demographics_geometry import DemographicsGeometry
 from com.precisely.apis.model.demographics_geometry_crc import DemographicsGeometryCRC
 from com.precisely.apis.model.demographics_themes_v2 import DemographicsThemesV2
 from com.precisely.apis.model.depth import Depth
-from com.precisely.apis.model.device_status_network import DeviceStatusNetwork
 from com.precisely.apis.model.direction_geometry import DirectionGeometry
 from com.precisely.apis.model.distance import Distance
 from com.precisely.apis.model.distance_to_border import DistanceToBorder
 from com.precisely.apis.model.distance_to_flood_hazard_address_request import DistanceToFloodHazardAddressRequest
 from com.precisely.apis.model.distance_to_flood_hazard_location_request import DistanceToFloodHazardLocationRequest
 from com.precisely.apis.model.distance_to_flood_hazard_response import DistanceToFloodHazardResponse
 from com.precisely.apis.model.district_type import DistrictType
@@ -136,15 +135,14 @@
 from com.precisely.apis.model.formatted_tax_address import FormattedTaxAddress
 from com.precisely.apis.model.foundation import Foundation
 from com.precisely.apis.model.free_or_reduced_price_lunches import FreeOrReducedPriceLunches
 from com.precisely.apis.model.fuel_type import FuelType
 from com.precisely.apis.model.garage_type import GarageType
 from com.precisely.apis.model.geo_location_access_point import GeoLocationAccessPoint
 from com.precisely.apis.model.geo_location_country import GeoLocationCountry
-from com.precisely.apis.model.geo_location_fixed_line_country import GeoLocationFixedLineCountry
 from com.precisely.apis.model.geo_location_ip_addr import GeoLocationIpAddr
 from com.precisely.apis.model.geo_location_place import GeoLocationPlace
 from com.precisely.apis.model.geo_location_state import GeoLocationState
 from com.precisely.apis.model.geo_pos import GeoPos
 from com.precisely.apis.model.geocode_address import GeocodeAddress
 from com.precisely.apis.model.geocode_preferences import GeocodePreferences
 from com.precisely.apis.model.geocode_request import GeocodeRequest
@@ -218,14 +216,15 @@
 from com.precisely.apis.model.poi_boundary_preferences import POIBoundaryPreferences
 from com.precisely.apis.model.poi_boundary_response import POIBoundaryResponse
 from com.precisely.apis.model.poiby_geometry_request import POIByGeometryRequest
 from com.precisely.apis.model.psap_response import PSAPResponse
 from com.precisely.apis.model.parent_business import ParentBusiness
 from com.precisely.apis.model.pbkey import Pbkey
 from com.precisely.apis.model.phone_verification import PhoneVerification
+from com.precisely.apis.model.phone_verification_output import PhoneVerificationOutput
 from com.precisely.apis.model.place import Place
 from com.precisely.apis.model.places_response import PlacesResponse
 from com.precisely.apis.model.poi import Poi
 from com.precisely.apis.model.poi_boundary import PoiBoundary
 from com.precisely.apis.model.poi_classification import PoiClassification
 from com.precisely.apis.model.poi_count import PoiCount
 from com.precisely.apis.model.poi_count_request import PoiCountRequest
@@ -350,14 +349,17 @@
 from com.precisely.apis.model.validate_mailing_address_response import ValidateMailingAddressResponse
 from com.precisely.apis.model.validate_mailing_address_uscanapi_input import ValidateMailingAddressUSCANAPIInput
 from com.precisely.apis.model.validate_mailing_address_uscanapi_input_row import ValidateMailingAddressUSCANAPIInputRow
 from com.precisely.apis.model.validate_mailing_address_uscanapi_options import ValidateMailingAddressUSCANAPIOptions
 from com.precisely.apis.model.validate_mailing_address_uscanapi_output import ValidateMailingAddressUSCANAPIOutput
 from com.precisely.apis.model.validate_mailing_address_uscanapi_request import ValidateMailingAddressUSCANAPIRequest
 from com.precisely.apis.model.validate_mailing_address_uscanapi_response import ValidateMailingAddressUSCANAPIResponse
+from com.precisely.apis.model.validate_phone_number_api_request import ValidatePhoneNumberAPIRequest
+from com.precisely.apis.model.validate_phone_number_api_request_input import ValidatePhoneNumberAPIRequestInput
+from com.precisely.apis.model.validate_phone_number_api_request_input_row import ValidatePhoneNumberAPIRequestInputRow
 from com.precisely.apis.model.water_body import WaterBody
 from com.precisely.apis.model.water_body_response import WaterBodyResponse
 from com.precisely.apis.model.zones_address import ZonesAddress
 from com.precisely.apis.model.zones_boundary_geometry import ZonesBoundaryGeometry
 from com.precisely.apis.model.zones_contact_details import ZonesContactDetails
 from com.precisely.apis.model.zones_geometry import ZonesGeometry
 from com.precisely.apis.model.zones_parent_business import ZonesParentBusiness
```

### Comparing `com.precisely.apis-14.0.1/com/precisely/apis/rest.py` & `com.precisely.apis-15.0.0/com/precisely/apis/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 14.0.0
+    The version of the OpenAPI document: 15.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `com.precisely.apis-14.0.1/com.precisely.apis.egg-info/SOURCES.txt` & `com.precisely.apis-15.0.0/com.precisely.apis.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
 com/precisely/apis/model/demographics.py
 com/precisely/apis/model/demographics_advanced_preferences.py
 com/precisely/apis/model/demographics_advanced_request.py
 com/precisely/apis/model/demographics_geometry.py
 com/precisely/apis/model/demographics_geometry_crc.py
 com/precisely/apis/model/demographics_themes_v2.py
 com/precisely/apis/model/depth.py
-com/precisely/apis/model/device_status_network.py
 com/precisely/apis/model/direction_geometry.py
 com/precisely/apis/model/distance.py
 com/precisely/apis/model/distance_to_border.py
 com/precisely/apis/model/distance_to_flood_hazard_address_request.py
 com/precisely/apis/model/distance_to_flood_hazard_location_request.py
 com/precisely/apis/model/distance_to_flood_hazard_response.py
 com/precisely/apis/model/district_type.py
@@ -165,15 +164,14 @@
 com/precisely/apis/model/formatted_tax_address.py
 com/precisely/apis/model/foundation.py
 com/precisely/apis/model/free_or_reduced_price_lunches.py
 com/precisely/apis/model/fuel_type.py
 com/precisely/apis/model/garage_type.py
 com/precisely/apis/model/geo_location_access_point.py
 com/precisely/apis/model/geo_location_country.py
-com/precisely/apis/model/geo_location_fixed_line_country.py
 com/precisely/apis/model/geo_location_ip_addr.py
 com/precisely/apis/model/geo_location_place.py
 com/precisely/apis/model/geo_location_state.py
 com/precisely/apis/model/geo_pos.py
 com/precisely/apis/model/geocode_address.py
 com/precisely/apis/model/geocode_preferences.py
 com/precisely/apis/model/geocode_request.py
@@ -240,14 +238,15 @@
 com/precisely/apis/model/owners.py
 com/precisely/apis/model/parent_business.py
 com/precisely/apis/model/pb_key_address_request.py
 com/precisely/apis/model/pb_key_response.py
 com/precisely/apis/model/pb_key_response_list.py
 com/precisely/apis/model/pbkey.py
 com/precisely/apis/model/phone_verification.py
+com/precisely/apis/model/phone_verification_output.py
 com/precisely/apis/model/place.py
 com/precisely/apis/model/places_response.py
 com/precisely/apis/model/poi.py
 com/precisely/apis/model/poi_boundary.py
 com/precisely/apis/model/poi_boundary_address_request.py
 com/precisely/apis/model/poi_boundary_location_request.py
 com/precisely/apis/model/poi_boundary_locations.py
@@ -379,14 +378,17 @@
 com/precisely/apis/model/validate_mailing_address_response.py
 com/precisely/apis/model/validate_mailing_address_uscanapi_input.py
 com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py
 com/precisely/apis/model/validate_mailing_address_uscanapi_options.py
 com/precisely/apis/model/validate_mailing_address_uscanapi_output.py
 com/precisely/apis/model/validate_mailing_address_uscanapi_request.py
 com/precisely/apis/model/validate_mailing_address_uscanapi_response.py
+com/precisely/apis/model/validate_phone_number_api_request.py
+com/precisely/apis/model/validate_phone_number_api_request_input.py
+com/precisely/apis/model/validate_phone_number_api_request_input_row.py
 com/precisely/apis/model/water_body.py
 com/precisely/apis/model/water_body_response.py
 com/precisely/apis/model/zones_address.py
 com/precisely/apis/model/zones_boundary_geometry.py
 com/precisely/apis/model/zones_contact_details.py
 com/precisely/apis/model/zones_geometry.py
 com/precisely/apis/model/zones_parent_business.py
```

### Comparing `com.precisely.apis-14.0.1/setup.py` & `com.precisely.apis-15.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-    Precisely APIs
-
-    Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
-
-    The version of the OpenAPI document: 12.0.1
-    Generated by: https://openapi-generator.tech
-"""
-
-
-from setuptools import setup, find_packages  # noqa: H301
-
-NAME = "com.precisely.apis"
-VERSION = "14.0.1"
-# To install the library, run the following
-#
-# python setup.py install
-#
-# prerequisite: setuptools
-# http://pypi.python.org/pypi/setuptools
-
-REQUIRES = [
-  "urllib3 >= 1.25.3",
-  "python-dateutil",
-]
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description="Precisely APIs",
-    author="Precisely APIs Support",
-    author_email="PreciselyAPIs-Support@precisely.com",
-    url="https://developer.precisely.com/",
-    keywords=["Precisely APIs"],
-    python_requires=">=3.6",
-    install_requires=REQUIRES,
-    packages=find_packages(exclude=["test", "tests"]),
-    include_package_data=True,
-    license="Apache 2.0",
-    long_description="""\
-    Enhance and enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs. """
-)
+"""
+    Precisely APIs
+
+    Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
+
+    The version of the OpenAPI document: 15.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+from setuptools import setup, find_packages  # noqa: H301
+
+NAME = "com.precisely.apis"
+VERSION = "15.0.0"
+# To install the library, run the following
+#
+# python setup.py install
+#
+# prerequisite: setuptools
+# http://pypi.python.org/pypi/setuptools
+
+REQUIRES = [
+  "urllib3 >= 1.25.3",
+  "python-dateutil",
+]
+
+setup(
+    name=NAME,
+    version=VERSION,
+    description="Precisely APIs",
+    author="Precisely APIs Support",
+    author_email="PreciselyAPIs-Support@precisely.com",
+    url="https://developer.precisely.com/",
+    keywords=["Precisely APIs"],
+    python_requires=">=3.6",
+    install_requires=REQUIRES,
+    packages=find_packages(exclude=["test", "tests"]),
+    include_package_data=True,
+    license="Apache 2.0",
+    long_description="""\
+    Enhance and enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs. """
+)
```

