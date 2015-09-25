Result
======

This is the result::

    PLAY ***************************************************************************
    
    TASK [setup] *******************************************************************
    ok: [froyo]
    
    TASK [ansible-var-test : include_vars] *****************************************
    ok: [froyo] => (item=/home/drybjed/src/projects/devel/roles/ansible-var-test/vars/other_main.yml)
    
    TASK [ansible-var-test : Debug the var] ****************************************
    ok: [froyo] => {
        "changed": false, 
        "var_wrapper": [
            {
                "key": "This is {# apt_sources_release #} string"
            }
        ]
    }
