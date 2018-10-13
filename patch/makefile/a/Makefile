CXXFLAGS=-std=c++11 -g3

libprimus_vk.so: primus_vk.cpp
	g++ $(CXXFLAGS) -I/usr/include/vulkan -shared -fPIC $^ -o $@

libnv_vulkan_wrapper.so: nv_vulkan_wrapper.cpp
	g++ $(CXXFLAGS) -I/usr/include/vulkan -shared -fPIC $^ -o $@

primus-vk-diag: primus_vk_diag.o
	g++ -g3 -o $@ $^ -lX11 -lvulkan -ldl
