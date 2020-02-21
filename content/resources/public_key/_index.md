---
title: public_key resource
resource: public_key
draft: false
aliases:
- /resource_public_key.html
resource_reference: false
robots: noindex, nofollow
resource_description_list:
- warning:
    shortcode: EOL_provisioning.md
- markdown: 'Use the **public_key** resource to create and delete public keys,

    including RSA, DSA, and .pem file keys.'
resource_new_in: null
handler_types: false
syntax_description: "The syntax for using the **public_key** resource in a recipe\
  \ is as\nfollows:\n\n``` ruby\npublic_key 'name' do\n  attribute 'value' # see properties\
  \ section below\n  ...\n  action :action # see actions section below\nend\n```"
syntax_code_block: null
syntax_properties_list:
- '`public_key` tells Chef Infra Client to use the `Chef::Provider::PublicKey` provider
  during a Chef Infra Client run'
- '`name` is the name of the resource block; when the `path` property is not specified
  as part of a recipe, `name` is also the name of the public key'
- '`attribute` is zero (or more) of the properties that are available for this resource'
- '`action` identifies which steps Chef Infra Client will take to bring the node into
  the desired state'
syntax_full_code_block: null
syntax_full_properties_list: null
syntax_shortcode: null
registry_key: false
nameless_apt_update: false
nameless_build_essential: false
resource_package_options: false
actions_list:
  :create:
    markdown: Default. Use to create an RSA public key.
  :delete:
    markdown: Use to delete an RSA public key.
  :nothing:
    shortcode: resources_common_actions_nothing.md
properties_list:
- property: format
  ruby_type: null
  required: false
  default_value: null
  new_in: null
  description_list:
  - markdown: 'Use to specify the format of a public key. Possible values: `pem`

      and `der`. Default value: `pem`.'
- property: ignore_failure
  ruby_type: true, false
  required: false
  default_value: 'false'
  new_in: null
  description_list:
  - markdown: Continue running a recipe if a resource fails for any reason.
- property: notifies
  ruby_type: Symbol, Chef::Resource\[String\]
  required: false
  default_value: null
  new_in: null
  description_list:
  - shortcode: resources_common_notification_notifies.md
  - markdown: ''
  - shortcode: resources_common_notification_timers.md
  - markdown: ''
  - shortcode: resources_common_notification_notifies_syntax.md
- property: path
  ruby_type: null
  required: false
  default_value: null
  new_in: null
  description_list:
  - markdown: The path to a public key.
- property: retries
  ruby_type: Integer
  required: false
  default_value: '0'
  new_in: null
  description_list:
  - markdown: The number of attempts to catch exceptions and retry the resource.
- property: retry_delay
  ruby_type: Integer
  required: false
  default_value: '2'
  new_in: null
  description_list:
  - markdown: The retry delay (in seconds).
- property: source_key
  ruby_type: null
  required: false
  default_value: null
  new_in: null
  description_list:
  - markdown: 'Use to copy a public key, but apply a different `format` and

      `password`. Use in conjunction with `source_key_pass_phrase` and

      `source_key_path`.'
- property: source_key_pass_phrase
  ruby_type: null
  required: false
  default_value: null
  new_in: null
  description_list:
  - markdown: 'The pass phrase for the public key. Use in conjunction with

      `source_key` and `source_key_path`.'
- property: source_key_path
  ruby_type: null
  required: false
  default_value: null
  new_in: null
  description_list:
  - markdown: 'The path to the public key. Use in conjunction with `source_key` and

      `source_key_pass_phrase`.'
- property: subscribes
  ruby_type: Symbol, Chef::Resource\[String\]
  required: false
  default_value: null
  new_in: null
  description_list:
  - shortcode: resources_common_notification_subscribes.md
  - markdown: ''
  - shortcode: resources_common_notification_timers.md
  - markdown: ''
  - shortcode: resources_common_notification_subscribes_syntax.md
properties_shortcode: null
properties_multiple_packages: false
resource_directory_recursive_directories: false
resources_common_atomic_update: false
properties_resources_common_windows_security: false
remote_file_prevent_re_downloads: false
remote_file_unc_path: false
ps_credential_helper: false
ruby_style_basics_chef_log: false
debug_recipes_chef_shell: false
template_requirements: false
resources_common_properties: false
resources_common_notification: false
resources_common_guards: false
common_resource_functionality_multiple_packages: false
resources_common_guard_interpreter: false
remote_directory_recursive_directories: false
common_resource_functionality_resources_common_windows_security: false
handler_custom: false
cookbook_file_specificity: false
unit_file_verification: false
examples_list: null

---