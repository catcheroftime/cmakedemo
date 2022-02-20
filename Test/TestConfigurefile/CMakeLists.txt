cmake_minimum_required(VERSION 3.10)
project(TestConfigurefile)

option(FOO_ENABLE "Enable Foo" ON)
if(FOO_ENABLE)
  set(FOO_STRING "foo")
endif()

configure_file(config.h.in config.h)