include(BCMTest)

find_package(boost_align)
find_package(boost_functional)
find_package(boost_atomic)

bcm_test_link_libraries(boost_smart_ptr
boost::align
boost::functional
boost::atomic
)

#  Boost.SmartPtr Library test Jamfile
#
#  Copyright (c) 2003-2013 Peter Dimov
#  Copyright (c) 2003 Dave Abrahams
#
#  Distributed under the Boost Software License, Version 1.0. (See
#  accompanying file LICENSE_1_0.txt or copy at
#  http://www.boost.org/LICENSE_1_0.txt)

# bring in rules for testing




















bcm_test(NAME smart_ptr_test SOURCES smart_ptr_test.cpp)
bcm_test(NAME shared_ptr_basic_test SOURCES shared_ptr_basic_test.cpp)
bcm_test(NAME shared_ptr_test SOURCES shared_ptr_test.cpp)
bcm_test(NAME weak_ptr_test SOURCES weak_ptr_test.cpp)
bcm_test(NAME weak_ptr_move_test SOURCES weak_ptr_move_test.cpp)
bcm_test(NAME shared_from_this_test SOURCES shared_from_this_test.cpp)
bcm_test(NAME get_deleter_test SOURCES get_deleter_test.cpp)
bcm_test(NAME intrusive_ptr_test SOURCES intrusive_ptr_test.cpp)
bcm_test(NAME intrusive_ptr_move_test SOURCES intrusive_ptr_move_test.cpp)
bcm_test(NAME intrusive_ref_counter_test SOURCES intrusive_ref_counter_test.cpp)
bcm_test(NAME atomic_count_test SOURCES atomic_count_test.cpp)
bcm_test(NAME lw_mutex_test SOURCES lw_mutex_test.cpp)
bcm_test(NAME shared_ptr_assign_fail SOURCES shared_ptr_assign_fail.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME shared_ptr_delete_fail SOURCES shared_ptr_delete_fail.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME shared_ptr_compare_fail SOURCES shared_ptr_compare_fail.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME shared_ptr_alloc2_test SOURCES shared_ptr_alloc2_test.cpp)
bcm_test(NAME pointer_cast_test SOURCES pointer_cast_test.cpp)
bcm_test(NAME cpp11_pointer_cast_test SOURCES cpp11_pointer_cast_test.cpp)
bcm_test(NAME pointer_to_other_test SOURCES pointer_to_other_test.cpp COMPILE_ONLY)
bcm_test(NAME auto_ptr_rv_test SOURCES auto_ptr_rv_test.cpp)
bcm_test(NAME shared_ptr_alias_test SOURCES shared_ptr_alias_test.cpp)
bcm_test(NAME shared_ptr_rv_test SOURCES shared_ptr_rv_test.cpp)
bcm_test(NAME shared_ptr_rv_pointer_cast_test SOURCES shared_ptr_rv_pointer_cast_test.cpp)
bcm_test(NAME shared_ptr_move_test SOURCES shared_ptr_move_test.cpp)
bcm_test(NAME shared_ptr_alias_move_test SOURCES shared_ptr_alias_move_test.cpp)
bcm_test(NAME shared_ptr_reinterpret_pointer_cast_test SOURCES shared_ptr_reinterpret_pointer_cast_test.cpp)
bcm_test(NAME shared_ptr_pv_fail SOURCES shared_ptr_pv_fail.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME sp_unary_addr_test SOURCES sp_unary_addr_test.cpp)
bcm_test(NAME scoped_ptr_eq_fail SOURCES scoped_ptr_eq_fail.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME scoped_array_eq_fail SOURCES scoped_array_eq_fail.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME esft_regtest SOURCES esft_regtest.cpp)
bcm_test(NAME yield_k_test SOURCES yield_k_test.cpp)
bcm_test(NAME yield_k_test.mt SOURCES yield_k_test.cpp)
bcm_test(NAME spinlock_test SOURCES spinlock_test.cpp)
bcm_test(NAME spinlock_try_test SOURCES spinlock_try_test.cpp)
bcm_test(NAME spinlock_try_test.mt SOURCES spinlock_try_test.cpp)
bcm_test(NAME spinlock_pool_test SOURCES spinlock_pool_test.cpp)
bcm_test(NAME make_shared_test SOURCES make_shared_test.cpp)
bcm_test(NAME make_shared_move_emulation_test SOURCES make_shared_move_emulation_test.cpp)
bcm_test(NAME make_shared_perfect_forwarding_test SOURCES make_shared_perfect_forwarding_test.cpp)
bcm_test(NAME shared_ptr_convertible_test SOURCES shared_ptr_convertible_test.cpp)
bcm_test(NAME wp_convertible_test SOURCES wp_convertible_test.cpp)
bcm_test(NAME ip_convertible_test SOURCES ip_convertible_test.cpp)
bcm_test(NAME allocate_shared_test SOURCES allocate_shared_test.cpp)
bcm_test(NAME sp_atomic_test SOURCES sp_atomic_test.cpp)
bcm_test(NAME esft_void_test SOURCES esft_void_test.cpp)
bcm_test(NAME esft_second_ptr_test SOURCES esft_second_ptr_test.cpp)
bcm_test(NAME make_shared_esft_test SOURCES make_shared_esft_test.cpp)
bcm_test(NAME allocate_shared_esft_test SOURCES allocate_shared_esft_test.cpp)
bcm_test(NAME sp_recursive_assign_test SOURCES sp_recursive_assign_test.cpp)
bcm_test(NAME sp_recursive_assign2_test SOURCES sp_recursive_assign2_test.cpp)
bcm_test(NAME sp_recursive_assign_rv_test SOURCES sp_recursive_assign_rv_test.cpp)
bcm_test(NAME sp_recursive_assign2_rv_test SOURCES sp_recursive_assign2_rv_test.cpp)
bcm_test(NAME auto_ptr_lv_fail SOURCES auto_ptr_lv_fail.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME atomic_count_test2 SOURCES atomic_count_test2.cpp)
bcm_test(NAME sp_typeinfo_test SOURCES sp_typeinfo_test.cpp)
bcm_test(NAME make_shared_fp_test SOURCES make_shared_fp_test.cpp COMPILE_ONLY)
bcm_test(NAME sp_hash_test SOURCES sp_hash_test.cpp)
bcm_test(NAME get_deleter_array_test SOURCES get_deleter_array_test.cpp)
bcm_test(NAME ip_hash_test SOURCES ip_hash_test.cpp)
bcm_test(NAME owner_less_test SOURCES owner_less_test.cpp)
bcm_test(NAME sp_unique_ptr_test SOURCES sp_unique_ptr_test.cpp)
bcm_test(NAME sp_array_test SOURCES sp_array_test.cpp)
bcm_test(NAME sp_array_cv_test SOURCES sp_array_cv_test.cpp COMPILE_ONLY)
bcm_test(NAME sp_convertible_test SOURCES sp_convertible_test.cpp)
bcm_test(NAME sp_array_n_test SOURCES sp_array_n_test.cpp)
bcm_test(NAME sp_array_cast_test SOURCES sp_array_cast_test.cpp)
bcm_test(NAME sp_zero_compare_test SOURCES sp_zero_compare_test.cpp)
bcm_test(NAME sp_nullptr_test SOURCES sp_nullptr_test.cpp)
bcm_test(NAME sa_nullptr_test SOURCES sa_nullptr_test.cpp)
bcm_test(NAME shared_ptr_alloc3_test SOURCES shared_ptr_alloc3_test.cpp)
bcm_test(NAME shared_ptr_alloc11_test SOURCES shared_ptr_alloc11_test.cpp)
bcm_test(NAME shared_ptr_alloc_construct11_test SOURCES shared_ptr_alloc_construct11_test.cpp)
bcm_test(NAME allocate_shared_alloc11_test SOURCES allocate_shared_alloc11_test.cpp)
bcm_test(NAME allocate_shared_construct11_test SOURCES allocate_shared_construct11_test.cpp)
bcm_test(NAME sp_interlocked_test SOURCES sp_interlocked_test.cpp)
bcm_test(NAME array_fail_spa_sp_c SOURCES array_fail_spa_sp_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_sp_spa_c SOURCES array_fail_sp_spa_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_spa_c SOURCES array_fail_spa_spa_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_wp_c SOURCES array_fail_spa_wp_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_sp_wpa_c SOURCES array_fail_sp_wpa_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_wpa_c SOURCES array_fail_spa_wpa_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wpa_wp_c SOURCES array_fail_wpa_wp_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wp_wpa_c SOURCES array_fail_wp_wpa_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wpa_wpa_c SOURCES array_fail_wpa_wpa_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_ap_spa_c SOURCES array_fail_ap_spa_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_upa_sp_c SOURCES array_fail_upa_sp_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_up_spa_c SOURCES array_fail_up_spa_c.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_sp_mc SOURCES array_fail_spa_sp_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_sp_spa_mc SOURCES array_fail_sp_spa_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_spa_mc SOURCES array_fail_spa_spa_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_wp_mc SOURCES array_fail_spa_wp_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_sp_wpa_mc SOURCES array_fail_sp_wpa_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_wpa_mc SOURCES array_fail_spa_wpa_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wpa_wp_mc SOURCES array_fail_wpa_wp_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wp_wpa_mc SOURCES array_fail_wp_wpa_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wpa_wpa_mc SOURCES array_fail_wpa_wpa_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_ap_spa_mc SOURCES array_fail_ap_spa_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_upa_sp_mc SOURCES array_fail_upa_sp_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_up_spa_mc SOURCES array_fail_up_spa_mc.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_sp_a SOURCES array_fail_spa_sp_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_sp_spa_a SOURCES array_fail_sp_spa_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_spa_a SOURCES array_fail_spa_spa_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_wp_a SOURCES array_fail_spa_wp_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_sp_wpa_a SOURCES array_fail_sp_wpa_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_wpa_a SOURCES array_fail_spa_wpa_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wpa_wp_a SOURCES array_fail_wpa_wp_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wp_wpa_a SOURCES array_fail_wp_wpa_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wpa_wpa_a SOURCES array_fail_wpa_wpa_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_ap_spa_a SOURCES array_fail_ap_spa_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_upa_sp_a SOURCES array_fail_upa_sp_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_up_spa_a SOURCES array_fail_up_spa_a.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_sp_ma SOURCES array_fail_spa_sp_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_sp_spa_ma SOURCES array_fail_sp_spa_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_spa_ma SOURCES array_fail_spa_spa_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_wp_ma SOURCES array_fail_spa_wp_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_sp_wpa_ma SOURCES array_fail_sp_wpa_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_spa_wpa_ma SOURCES array_fail_spa_wpa_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wpa_wp_ma SOURCES array_fail_wpa_wp_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wp_wpa_ma SOURCES array_fail_wp_wpa_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_wpa_wpa_ma SOURCES array_fail_wpa_wpa_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_ap_spa_ma SOURCES array_fail_ap_spa_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_upa_sp_ma SOURCES array_fail_upa_sp_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_up_spa_ma SOURCES array_fail_up_spa_ma.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_dereference SOURCES array_fail_dereference.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_member_access SOURCES array_fail_member_access.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME array_fail_array_access SOURCES array_fail_array_access.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME make_shared_array_test SOURCES make_shared_array_test.cpp)
bcm_test(NAME make_shared_arrays_test SOURCES make_shared_arrays_test.cpp)
bcm_test(NAME make_shared_array_throws_test SOURCES make_shared_array_throws_test.cpp)
bcm_test(NAME make_shared_array_esft_test SOURCES make_shared_array_esft_test.cpp)
bcm_test(NAME make_shared_array_noinit_test SOURCES make_shared_array_noinit_test.cpp)
bcm_test(NAME make_shared_array_value_test SOURCES make_shared_array_value_test.cpp)
bcm_test(NAME allocate_shared_array_test SOURCES allocate_shared_array_test.cpp)
bcm_test(NAME allocate_shared_arrays_test SOURCES allocate_shared_arrays_test.cpp)
bcm_test(NAME allocate_shared_array_throws_test SOURCES allocate_shared_array_throws_test.cpp)
bcm_test(NAME allocate_shared_array_esft_test SOURCES allocate_shared_array_esft_test.cpp)
bcm_test(NAME allocate_shared_array_noinit_test SOURCES allocate_shared_array_noinit_test.cpp)
bcm_test(NAME allocate_shared_array_value_test SOURCES allocate_shared_array_value_test.cpp)
bcm_test(NAME allocate_shared_array_construct_test SOURCES allocate_shared_array_construct_test.cpp)
bcm_test(NAME make_unique_test SOURCES make_unique_test.cpp)
bcm_test(NAME make_unique_args_test SOURCES make_unique_args_test.cpp)
bcm_test(NAME make_unique_value_test SOURCES make_unique_value_test.cpp)
bcm_test(NAME make_unique_noinit_test SOURCES make_unique_noinit_test.cpp)
bcm_test(NAME make_unique_throws_test SOURCES make_unique_throws_test.cpp)
bcm_test(NAME make_unique_array_test SOURCES make_unique_array_test.cpp)
bcm_test(NAME make_unique_array_noinit_test SOURCES make_unique_array_noinit_test.cpp)
bcm_test(NAME make_unique_array_throws_test SOURCES make_unique_array_throws_test.cpp)
bcm_test(NAME shared_from_raw_test SOURCES shared_from_raw_test.cpp)
bcm_test(NAME shared_from_raw_test2 SOURCES shared_from_raw_test2.cpp)
bcm_test(NAME shared_from_raw_test3 SOURCES shared_from_raw_test3.cpp)
bcm_test(NAME shared_from_raw_test4 SOURCES shared_from_raw_test4.cpp)
bcm_test(NAME shared_from_raw_test5 SOURCES shared_from_raw_test5.cpp)
bcm_test(NAME shared_from_raw_test6 SOURCES shared_from_raw_test6.cpp)
bcm_test(NAME weak_from_raw_test SOURCES weak_from_raw_test.cpp)
bcm_test(NAME weak_from_raw_test2 SOURCES weak_from_raw_test2.cpp)
bcm_test(NAME weak_from_raw_test3 SOURCES weak_from_raw_test3.cpp)
bcm_test(NAME weak_from_raw_test4 SOURCES weak_from_raw_test4.cpp)
bcm_test(NAME weak_from_raw_test5 SOURCES weak_from_raw_test5.cpp)
bcm_test(NAME sp_explicit_inst_test SOURCES sp_explicit_inst_test.cpp COMPILE_ONLY)
bcm_test(NAME weak_from_this_test SOURCES weak_from_this_test.cpp)
bcm_test(NAME weak_from_this_test2 SOURCES weak_from_this_test2.cpp)
bcm_test(NAME sp_bml_unique_ptr_test SOURCES sp_bml_unique_ptr_test.cpp)
bcm_test(NAME sp_hash_test2 SOURCES sp_hash_test2.cpp)
bcm_test(NAME sp_hash_test3 SOURCES sp_hash_test3.cpp)
bcm_test(NAME pointer_cast_test2 SOURCES pointer_cast_test2.cpp)
bcm_test(NAME pointer_cast_st_fail SOURCES pointer_cast_st_fail.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME pointer_cast_st_fail2 SOURCES pointer_cast_st_fail2.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME pointer_cast_st_fail3 SOURCES pointer_cast_st_fail3.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME pointer_cast_co_fail SOURCES pointer_cast_co_fail.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME pointer_cast_co_fail2 SOURCES pointer_cast_co_fail2.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME pointer_cast_co_fail3 SOURCES pointer_cast_co_fail3.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME pointer_cast_dy_fail SOURCES pointer_cast_dy_fail.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME pointer_cast_dy_fail2 SOURCES pointer_cast_dy_fail2.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME pointer_cast_dy_fail3 SOURCES pointer_cast_dy_fail3.cpp COMPILE_ONLY WILL_FAIL)
bcm_test(NAME sp_nothrow_test SOURCES sp_nothrow_test.cpp)
bcm_test(NAME make_shared_msvc_test SOURCES make_shared_msvc_test.cpp COMPILE_ONLY)

