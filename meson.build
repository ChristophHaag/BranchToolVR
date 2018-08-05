project(
	'branchtoolvr', 'cpp',
	default_options : 'cpp_std=c++11',
)
sources = [
	'BranchToolVR/AbstractBaseObject.cpp',
	'BranchToolVR/CoarseDicomViewer.cpp',
	'BranchToolVR/ColorObject.cpp',
	'BranchToolVR/Curve.cpp',
	'BranchToolVR/DicomObjectsContainer.cpp',
	'BranchToolVR/DicomPointCloudObject.cpp',
	'BranchToolVR/DicomReader.cpp',
	'BranchToolVR/Engine.cpp',
	'BranchToolVR/InputHelpers.cpp',
	'BranchToolVR/LeastSquaresFit.cpp',
	'BranchToolVR/LineObject.cpp',
	'BranchToolVR/MarchingCubesVars.cpp',
	'BranchToolVR/Render.cpp',
	'BranchToolVR/RenderModel.cpp',
	'BranchToolVR/Texture.cpp',
	'BranchToolVR/TextureObject.cpp',
	'BranchToolVR/imgui_impl_glfw_gl3.cpp',
	'BranchToolVR/main.cpp'
]

glm_dep = dependency('glm')

args = ['-DLINUX']

inc = include_directories([
	'BranchToolVR',
	'BranchToolVR/Libraries/imgui',
	'BranchToolVR/Libraries/misc/',
	'BranchToolVR/Libraries/imebra/library/imebra/include/'
])

deps = [glm_dep]

executable('branchtoolvr', sources, include_directories : inc, install : true, dependencies : deps, cpp_args : args)
