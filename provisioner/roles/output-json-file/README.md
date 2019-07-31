---
- name: "Output the value of input_json to {{ output_path }}"
  template:
    src:        output_json.j2
    dest:       "{{ output_file }}"

- name: Print the value of input_json
  debug:
    var:        input_json
    verbosity:  2
