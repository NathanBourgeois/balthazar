# Setup your environment

The steps to build this project is setup a Zephyr environment in your computer and then get the project

1. Create a workspace directory (such as workspace)
2. Follow the instruction of Zephyr getting started guide (https://docs.zephyrproject.org/latest/develop/getting_started/index.html)
	* Install dependencies
	* Get Zephyr and install Python dependencies
3. In your workspace directory, activate the virtual environment
4. west init -m git@github.com:NathanBourgeois/balthazar.git --mr main balthazar
5. cd balthazar
6. west update
7. cd zephyr
8. west sdk install

Now your computer is setup to build the project, you don't need to repeat those step *except* for activating the virtual environment.

# How to build

west build -p -b promicro app

# How to DFU

I use the recommanded software AuTerm as indicated in the Nordic Academy : https://academy.nordicsemi.com/courses/nrf-connect-sdk-intermediate/lessons/lesson-9-bootloaders-and-dfu-fota/topic/exercise-1-dfu-over-uart/#serial_recovery
