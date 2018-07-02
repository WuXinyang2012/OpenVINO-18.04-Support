#Xinyang Wu   
In fact, the only difference between Ubuntu 16.04 and 18.04 is that two required modules: libpng12 and libgstream0.10 are not supported in Ubuntu 18.04, instead are libpng16 and libgstream1.0. You can just comment those two unsupported modules yourself in any scripts you want to run.


# Unofficial Ubuntu 18.04 Support for OpenVINO™

As of June 2018, OpenVINO™ only supports Ubuntu 16.04.3 LTS (64 bit), Windows 10 (64 bit) and CentOS 7.4 (64 bit). James Lim (@jameshi16) and I have modified the `InferenceEngineConfig.cmake` to allow OpenVINO™ to run on Ubuntu 18.04 without any issues.

## How to use it

Replace and run the shell script `/opt/intel/computer_vision_sdk_2018.1.265/deployment_tools/inference_engine/share/InferenceEngineConfig.cmake` with the `InferenceEngineConfig.cmake` provided in this repository.

To test if you have sucessfully installed and configured OpenVINO on your host, replace and run the `demo_squeezenet_download_convert_run.sh` with the one provided in this repository at this location: `/opt/intel/computer_vision_sdk_2018.1.265/deployment_tools/demo`.

# Contributors

Nikhil Raghavendra (@nikhilraghava) and James Lim (@jameshi16).

Copyright © Intel Corporation. Licensed under the Apache License, Version 2.0.
