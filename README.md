Based on steps from https://wiki.archlinux.org/title/Hybrid_graphics#Fully_power_down_discrete_GPU and meant to be used with the proprietary nvidia drivers.

`gpu off` will disable the nvidia gpu with udev rules and disable the nvidia-persistenced service.

`gpu on` will re-enable the nvidia gpu by removing the rules disabling it.

A reboot is required for changes to take affect.

Why would you use this? If you have a gaming laptop, even with optimus (hybrid) graphics, the battery life may still be abysmal only lasting 1-2 hours. Turning the dedicated gpu off in my experience can stretch that to 6+ hours.
