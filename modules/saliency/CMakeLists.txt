if(CV_ICC AND NOT MSVC)
  ocv_module_disable(saliency)
endif()

set(the_description "Saliency API")
set(OPENCV_MODULE_IS_PART_OF_WORLD OFF)

ocv_define_module(saliency opencv_imgproc opencv_highgui opencv_features2d WRAP python)

ocv_warnings_disable(CMAKE_CXX_FLAGS -Woverloaded-virtual)
