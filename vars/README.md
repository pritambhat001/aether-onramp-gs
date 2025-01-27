# OnRamp Variables

File `main.yml` specifies global variables used to configure how Aether is deployed.
By default, it is configured for the Quick Start deployment. The other files define
common configurations, any one of which you can copy to `main.yml`, and then
edit to account for your local details. These alternative configurations include:

* `main-quickstart.yml`: Configures the RAN emulator (gNBsim) to run in the same
   server as the Core. Equivalent to `main.yml` by default.

* `main-gnbsim.yml`: Configures the RAN emulator (gNBsim) to run in one or more
   servers, independent of the Core.

* `main-gNB.yml`: Configures the Core to work with an external 5G radio (gNB), with 
   the Core running independent of AMP. (Change variable `standalone` to false to have
   the Core running under AMP's control.)

* `main-eNB.yml`: Configures the Core to work with an external 4G radio (eNB), with 
   the Core running independent of AMP. (Change variable `standalone` to false to have 
   the Core running under AMP's control.)
