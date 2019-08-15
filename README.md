#hardware/qcom/display/msm8974/libcopybit/copybit_c2d.cpp

Error: "android.hardware.power@1.1-service-qti (EXECUTABLES android-arm) missing vendor.lineage.power@1.0 (SHARED_LIBRARIES android-arm)"

add: git clone https://github.com/LineageOS/android_hardware_lineage_interfaces -b lineage-16.0 hardware/lineage/interfaces and delete "hardware/custom" folder.

//////

Modifications required:
https://github.com/LineageOS/android_hardware_qcom_display/commit/e22306c18af7dfeea279b1135adf292144139c4e  ( in hardware/qcom/display/msm8974 )
and clone this too..
git clone https://github.com/LineageOS/android_packages_resources_devicesettings -b lineage-16.0 packages/resources/devicesettings

//////
Out of space?

#BoardConfig.mk
TARGET_MINIMAL_APPS := true

