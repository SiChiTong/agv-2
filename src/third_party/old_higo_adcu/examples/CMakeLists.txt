cmake_minimum_required(VERSION 3.5)
project (adcuExamples)

link_directories(../lib)
include_directories(../include)

#add_executable (samples main.cpp)
#target_link_libraries(samples WiseADCUSdk pthread)

add_executable(can_test can_test.cpp)
add_executable(adc_test adc_test.cpp)
add_executable(dac_test dac_test.cpp)
add_executable(lin_test lin_test.cpp)
add_executable(highside_test highside_test.cpp)
add_executable(power_test power_test.cpp)
add_executable(pwm_in_test pwm_in_test.cpp)
add_executable(pwm_out_test pwm_out_test.cpp)
add_executable(rs232_test rs232_test.cpp)
add_executable(rs485_test rs485_test.cpp)

target_link_libraries(can_test WiseADCUSdk pthread)
target_link_libraries(adc_test WiseADCUSdk pthread)
target_link_libraries(dac_test WiseADCUSdk pthread)
target_link_libraries(lin_test WiseADCUSdk pthread)
target_link_libraries(highside_test WiseADCUSdk pthread)
target_link_libraries(power_test WiseADCUSdk pthread)
target_link_libraries(pwm_in_test WiseADCUSdk pthread)
target_link_libraries(pwm_out_test WiseADCUSdk pthread)
target_link_libraries(rs232_test WiseADCUSdk pthread)
target_link_libraries(rs485_test WiseADCUSdk pthread)
