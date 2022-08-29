cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(SequenceTransformer)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/SequenceTransformer")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "Chris (Gibson)")
set(EXTENSION_DESCRIPTION "A 3D Slicer module used to create copies of transformed nodes at certain time points within a sequence.")
set(EXTENSION_ICONURL "https://www.example.com/Slicer/Extensions/SequenceTransformer.png")
set(EXTENSION_SCREENSHOTURLS "https://www.example.com/Slicer/Extensions/SequenceTransformer/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(SequenceTransformer)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
