caffe
=====

[Caffe](http://caffe.berkeleyvision.org/) installation role for ansible

Requirements
------------

opencv >= 3.1.0 & opencv-contrib >= 3.1.0, both installed using role beeva-mariorodriguez/ansible-opencv

Role Variables
--------------

* ``enable_cuda``: require NVIDIA CUDA drivers, default: false (CPU-only installation)
* ``blas``: install ATLAS or OpenBLAS, default: "ATLAS"
* ``caffe_version``: default: "1.0"
* ``reinstall``: overwrite current installation (default: False)
* ``delete_sources``: delete sources after installation (default: False)

Dependencies
------------

none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: caffe
      roles:
         - { role: opencv }
         - { role: caffe, blas: "OpenBLAS", enable_cuda: false }

License
-------

BSD

Author Information
------------------

Mario Rodríguez

