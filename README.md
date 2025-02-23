README for running visualization code for the following publication:

@article{mcgee2020generative,
  title={Generative Capacity of Probabilistic Protein Sequence Models},
  author={McGee, Francisco and Novinger, Quentin and Levy, Ronald M and Carnevale, Vincenzo and Haldane, Allan},
  journal={arXiv preprint arXiv:2012.02296},
  year={2020}
}

This code is for computing, and generating visualizations of, 
generative capacity metrics for MSAs generated by 
generative protein sequence models (GPSMs).

Visualization parameters are all in the JSON config file, so
that will need to be edited prior to individual use. Such
parameters include typographical settings (font sizes, etc) 
and which visualizations to run, but most critically, 
the paths for the MSA datasets on which the metrics are to be computed.

After configuring the JSON file appropriately,
the generative capacityh metrics can be computed and visualized 
by calling the controller script on the config file as follows::

```
cd mi3gpu/utils && make
python controller.py config_vis.json
```

# TODO
- FileNotFoundError: [Errno 2] No such file or directory: 'example/nat_filt_0.5_10K_target'

