# NVIDIA_FLARE Short Q&A: 


Here you can find a short Q&A, in particular, those questions I had when tesing this framework, and could not see a clear answer in the official documentation.
Please, let me know if there are some more I should add. :)

1. Is it possible to run 2 experiments at the same time? 

No, Flare (below 2.1) does not support this option. When trying to run 2 experiments, one will get an error "Server already starting or started". One needs to wait till the current experiment finishes, then an app can be launched.

2. Is Flare 2.0 compatible with Flare 2.1?

No, due to API version 3.0 in Flare 2.1 and older versions in Flare 2.0. The Provision Tool has been enhanced to support some configurations of additional components.
