LIB = libgponctl.so
default: dynamic


libgponctl.so:
	cp libgponctl.so_$(PROFILE)_save libgponctl.so

dynamic: generic_private_lib_install

clean:
	rm -f libgponctl.so

CURR_DIR := $(shell pwd)
BUILD_DIR := $(subst /userspace, /userspace,$(CURR_DIR))
BUILD_DIR := $(word 1, $(BUILD_DIR))
include $(BUILD_DIR)/make.common
