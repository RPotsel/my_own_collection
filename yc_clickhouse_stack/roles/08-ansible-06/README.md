08-ansible-06
=========

Creates a file with the contents at the specified path.

Requirements
------------

None

Role Variables
--------------

  - `file_path`: path to file
  - `file_content`: content the file

Dependencies
------------

git@github.com:rpotsel/my_own_collection.git

Example Playbook
----------------

  ```YAML
  - name: Testing collection playbook
    hosts: localhost
    collections:
      - my_own_collection.yc_clickhouse_stack
    vars:
      - file_path: "./test_collection.txt"
      - file_content: "Test collection"
    roles:
      - 08-ansible-06
   ```

License
-------

MIT

