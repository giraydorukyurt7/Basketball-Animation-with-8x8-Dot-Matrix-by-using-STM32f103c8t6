################################################################################
# Automatically-generated file. Do not edit!
# Toolchain: GNU Tools for STM32 (11.3.rel1)
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32F1xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(S_DEPS)),)
-include $(S_DEPS)
endif
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

OPTIONAL_TOOL_DEPS := \
$(wildcard ../makefile.defs) \
$(wildcard ../makefile.init) \
$(wildcard ../makefile.targets) \


BUILD_ARTIFACT_NAME := Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6
BUILD_ARTIFACT_EXTENSION := elf
BUILD_ARTIFACT_PREFIX :=
BUILD_ARTIFACT := $(BUILD_ARTIFACT_PREFIX)$(BUILD_ARTIFACT_NAME)$(if $(BUILD_ARTIFACT_EXTENSION),.$(BUILD_ARTIFACT_EXTENSION),)

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.elf \

MAP_FILES += \
Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.map \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.list \

OBJCOPY_HEX += \
Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.hex \

OBJCOPY_BIN += \
Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.bin \


# All Target
all: main-build

# Main-build Target
main-build: Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.elf secondary-outputs

# Tool invocations
Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.elf Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.map: $(OBJS) $(USER_OBJS) C:\Users\Giray\STM32CubeIDE\workspace_1.14.1\Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6\STM32F103C8TX_FLASH.ld makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-gcc -o "Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m3 -T"C:\Users\Giray\STM32CubeIDE\workspace_1.14.1\Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6\STM32F103C8TX_FLASH.ld" --specs=nosys.specs -Wl,-Map="Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.map" -Wl,--gc-sections -static --specs=nano.specs -mfloat-abi=soft -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.list: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.list"
	@echo 'Finished building: $@'
	@echo ' '

Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.hex: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-objcopy  -O ihex $(EXECUTABLES) "Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.hex"
	@echo 'Finished building: $@'
	@echo ' '

Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.bin: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.bin"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.bin Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.elf Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.hex Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.list Project_1_8x8_Dot_Matrix_Heart_Shape_With_Stm32f103c8t6.map default.size.stdout
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST) $(OBJCOPY_HEX) $(OBJCOPY_BIN)

fail-specified-linker-script-missing:
	@echo 'Error: Cannot find the specified linker script. Check the linker settings in the build configuration.'
	@exit 2

warn-no-linker-script-specified:
	@echo 'Warning: No linker script specified. Check the linker settings in the build configuration.'

.PHONY: all clean dependents main-build fail-specified-linker-script-missing warn-no-linker-script-specified

-include ../makefile.targets
