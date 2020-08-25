RM = rm -f

APPDIR = ${shell pwd}
-include $(TOPDIR)/Make.defs



#SRCS := \
#tensorflow/lite/micro/simple_memory_allocator.cc tensorflow/lite/micro/memory_helpers.cc tensorflow/lite/micro/test_helpers.cc tensorflow/lite/micro/micro_error_reporter.cc tensorflow/lite/micro/micro_time.cc tensorflow/lite/micro/debug_log.cc tensorflow/lite/micro/micro_string.cc tensorflow/lite/micro/micro_utils.cc tensorflow/lite/micro/micro_optional_debug_tools.cc tensorflow/lite/micro/micro_interpreter.cc tensorflow/lite/micro/micro_allocator.cc tensorflow/lite/micro/kernels/logical.cc tensorflow/lite/micro/kernels/elementwise.cc tensorflow/lite/micro/kernels/comparisons.cc tensorflow/lite/micro/kernels/depthwise_conv.cc tensorflow/lite/micro/kernels/split.cc tensorflow/lite/micro/kernels/logistic.cc tensorflow/lite/micro/kernels/circular_buffer.cc tensorflow/lite/micro/kernels/prelu.cc tensorflow/lite/micro/kernels/softmax.cc tensorflow/lite/micro/kernels/dequantize.cc tensorflow/lite/micro/kernels/neg.cc tensorflow/lite/micro/kernels/pack.cc tensorflow/lite/micro/kernels/activations.cc tensorflow/lite/micro/kernels/ceil.cc tensorflow/lite/micro/kernels/arg_min_max.cc tensorflow/lite/micro/kernels/unpack.cc tensorflow/lite/micro/kernels/fully_connected.cc tensorflow/lite/micro/kernels/add.cc tensorflow/lite/micro/kernels/floor.cc tensorflow/lite/micro/kernels/pooling.cc tensorflow/lite/micro/kernels/concatenation.cc tensorflow/lite/micro/kernels/conv.cc tensorflow/lite/micro/kernels/svdf.cc tensorflow/lite/micro/kernels/quantize.cc tensorflow/lite/micro/kernels/all_ops_resolver.cc tensorflow/lite/micro/kernels/pad.cc tensorflow/lite/micro/kernels/mul.cc tensorflow/lite/micro/kernels/maximum_minimum.cc tensorflow/lite/micro/kernels/reshape.cc tensorflow/lite/micro/kernels/reduce.cc tensorflow/lite/micro/kernels/strided_slice.cc tensorflow/lite/micro/kernels/round.cc tensorflow/lite/micro/memory_planner/linear_memory_planner.cc tensorflow/lite/micro/memory_planner/greedy_memory_planner.cc tensorflow/lite/c/common.c tensorflow/lite/core/api/error_reporter.cc tensorflow/lite/core/api/flatbuffer_conversions.cc tensorflow/lite/core/api/op_resolver.cc tensorflow/lite/core/api/tensor_utils.cc tensorflow/lite/kernels/internal/quantization_util.cc tensorflow/lite/kernels/kernel_util.cc tensorflow/lite/micro/testing/test_utils.cc  tensorflow/lite/micro/examples/mnist/main.cc tensorflow/lite/micro/examples/mnist/main_functions.cc tensorflow/lite/micro/examples/mnist/output_handler.cc

SRCS := \
tensorflow/lite/micro/simple_memory_allocator.cc tensorflow/lite/micro/memory_helpers.cc tensorflow/lite/micro/test_helpers.cc tensorflow/lite/micro/micro_error_reporter.cc tensorflow/lite/micro/micro_time.cc tensorflow/lite/micro/debug_log.cc tensorflow/lite/micro/micro_string.cc tensorflow/lite/micro/micro_utils.cc tensorflow/lite/micro/micro_optional_debug_tools.cc tensorflow/lite/micro/micro_interpreter.cc tensorflow/lite/micro/micro_allocator.cc tensorflow/lite/micro/kernels/logical.cc tensorflow/lite/micro/kernels/elementwise.cc tensorflow/lite/micro/kernels/comparisons.cc tensorflow/lite/micro/kernels/depthwise_conv.cc tensorflow/lite/micro/kernels/split.cc tensorflow/lite/micro/kernels/logistic.cc tensorflow/lite/micro/kernels/circular_buffer.cc tensorflow/lite/micro/kernels/prelu.cc tensorflow/lite/micro/kernels/softmax.cc tensorflow/lite/micro/kernels/dequantize.cc tensorflow/lite/micro/kernels/neg.cc tensorflow/lite/micro/kernels/pack.cc tensorflow/lite/micro/kernels/activations.cc tensorflow/lite/micro/kernels/ceil.cc tensorflow/lite/micro/kernels/arg_min_max.cc tensorflow/lite/micro/kernels/unpack.cc tensorflow/lite/micro/kernels/fully_connected.cc tensorflow/lite/micro/kernels/add.cc tensorflow/lite/micro/kernels/floor.cc tensorflow/lite/micro/kernels/pooling.cc tensorflow/lite/micro/kernels/concatenation.cc tensorflow/lite/micro/kernels/conv.cc tensorflow/lite/micro/kernels/svdf.cc tensorflow/lite/micro/kernels/quantize.cc tensorflow/lite/micro/kernels/all_ops_resolver.cc tensorflow/lite/micro/kernels/pad.cc tensorflow/lite/micro/kernels/mul.cc tensorflow/lite/micro/kernels/maximum_minimum.cc tensorflow/lite/micro/kernels/reshape.cc tensorflow/lite/micro/kernels/reduce.cc tensorflow/lite/micro/kernels/strided_slice.cc tensorflow/lite/micro/kernels/round.cc tensorflow/lite/micro/memory_planner/linear_memory_planner.cc tensorflow/lite/micro/memory_planner/greedy_memory_planner.cc tensorflow/lite/c/common.c tensorflow/lite/core/api/error_reporter.cc tensorflow/lite/core/api/flatbuffer_conversions.cc tensorflow/lite/core/api/op_resolver.cc tensorflow/lite/core/api/tensor_utils.cc tensorflow/lite/kernels/internal/quantization_util.cc tensorflow/lite/kernels/kernel_util.cc tensorflow/lite/micro/testing/test_utils.cc tensorflow/lite/micro/examples/mnist/main_functions.cc tensorflow/lite/micro/examples/mnist/nxhello_bkgd.c tensorflow/lite/micro/examples/mnist/nxhello_listener.c tensorflow/lite/micro/examples/mnist/nxhello_main.c tensorflow/lite/micro/examples/mnist/nximage_bitmap.c tensorflow/lite/micro/examples/mnist/nximage_bkgd.c 

OBJS := \
$(patsubst %.cc,%.o,$(patsubst %.c,%.o,$(SRCS)))
  
ROOTDEPPATH = --dep-path .

#CXXFLAGS += -std=c++11 -DTF_LITE_STATIC_MEMORY -DCONFIG_LIBC_LOCALTIME -O3 -DCONFIG_LIBC_WCHAR -I. -I./third_party/gemmlowp -I./third_party/flatbuffers/include -I/home/jpdz/nuttx/code/nuttx/nuttx/include/libcxx -nostdinc++

CXXFLAGS += -std=c++11 -DTF_LITE_STATIC_MEMORY -D__NuttX__ -DCONFIG_LIBC_LOCALTIME -O3 -DCONFIG_LIBC_WCHAR -I. -I./third_party/gemmlowp -I./third_party/flatbuffers/include -I/home/jpdz/nuttx/code/nuttx/nuttx/include/libcxx -nostdinc++

#CXXFLAGS += -std=c++11 -DTF_LITE_STATIC_MEMORY -O3 -I. -I./third_party/gemmlowp -I./third_party/flatbuffers/include -I./third_party/kissfft -I/home/jpdz/nuttx/code/nuttxnew/nuttx/include/uClibc++ -I/home/jpdz/nuttx/code/nuttxnew/nuttx/include/cxx -nostdinc++ 

#CXXFLAGS += -std=c++11 -DTF_LITE_STATIC_MEMORY -O3 -I. -I./third_party/gemmlowp -I./third_party/flatbuffers/include -I./third_party/kissfft -I/home/jpdz/nuttx/gcc-arm-none-eabi-9-2019-q4-major-x86_64-linux/gcc-arm-none-eabi-9-2019-q4-major/arm-none-eabi/include/c++/9.2.1

#CXXFLAGS += -std=c++11 -DTF_LITE_STATIC_MEMORY -O3 -I. -I./third_party/gemmlowp -I./third_party/flatbuffers/include -I./third_party/kissfft -I/home/jpdz/nuttx/code/nuttxnew/buildroot/build_arm_hf/staging_dir/arm-nuttx-eabi/include/uClibc++

CFLAGS +=  -std=c11   -DTF_LITE_STATIC_MEMORY -O3 -I. -I./third_party/gemmlowp -I./third_party/flatbuffers/include -I/home/jpdz/nuttx/code/nuttx/nuttx/include/libcxx -I./third_party/kissfft -nostdinc

$(warning $(CXXFLAGS))

#LDFLAGS +=  -lm

%.o: %.cc
	$(CXX) $(CXXFLAGS) -c $< -o $@ 

%.o: %.c 
	$(CC) $(CFLAGS)  -c $< -o $@

libapps.a: $(OBJS)
	$(call ARCHIVE, libapps.a, $(OBJS))

all: libapps.a
.PHONY: dirlinks context preconfig depend clean clean_context distclean
.PRECIOUS: libapps$(LIBEXT)

# Create directory links
 
dirlinks:
 
# Setup any special pre-build context
 
context:
 
# Setup any special pre-configuration context
 
preconfig:
 
# Make the dependency file, Make.deps
 
.depend: Makefile $(SRCS)
	$(Q) $(MKDEP) $(ROOTDEPPATH) "$(CC)" -- $(CFLAGS) -- $(SRCS) >Make.dep
	$(Q) $(MKDEP) $(ROOTDEPPATH) "$(CXX)" -- $(CXXFLAGS) -- $(SRCS) >Make.dep
 
# Clean the results of the last build
 
clean: 
	$(call CLEAN)
 
# Remove the build context and directory links
 
clean_context:
 
# Restore the directory to its original state
 
distclean: clean clean_context
	$(call DELFILE, Make.dep)
	$(call DELFILE, .depend)

 
# Include dependencies
     
-include Make.dep
