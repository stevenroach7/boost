include(BCMTest)


bcm_test_link_libraries(boost_functional
)

#~ Copyright Rene Rivera 2008
#~ Distributed under the Boost Software License, Version 1.0.
#~ (See accompanying file LICENSE_1_0.txt or copy at http://www.boost.org/LICENSE_1_0.txt)


bcm_test(NAME function_test SOURCES function_test.cpp)

