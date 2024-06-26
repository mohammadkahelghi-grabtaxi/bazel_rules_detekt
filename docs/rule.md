<!-- Generated with Stardoc: http://skydoc.bazel.build -->

# Attributes

Name           | Type                               | Default            | Description
---------------|------------------------------------|--------------------|------------
`name` | [`name`](https://docs.bazel.build/versions/master/build-ref.html#name) | — | A unique name for this target.
`baseline` | [`Label`](https://docs.bazel.build/versions/master/skylark/lib/Label.html) | `None` | [Detekt baseline file](https://detekt.github.io/detekt/baseline.html).
`build_upon_default_config` | [`bool`](https://docs.bazel.build/versions/master/skylark/lib/bool.html) | `False` | See [Detekt `--build-upon-default-config` option](https://detekt.github.io/detekt/cli.html).
`auto_correct` | [`bool`](https://docs.bazel.build/versions/master/skylark/lib/bool.html) | `False` | See [Detekt `auto_correct` option](https://detekt.github.io/detekt/cli.html).
`disable_default_rule_sets` | [`bool`](https://docs.bazel.build/versions/master/skylark/lib/bool.html) | `False` | See [Detekt `disable_default_rule_sets` option](https://detekt.github.io/detekt/cli.html).
`all_rules` | [`bool`](https://docs.bazel.build/versions/master/skylark/lib/bool.html) | `False` | See [Detekt `all_rules` option](https://detekt.github.io/detekt/cli.html).
`cfgs` | [`[Label]`](https://docs.bazel.build/versions/master/skylark/lib/list.html) | `[]` | [Detekt configuration files](https://detekt.github.io/detekt/configurations.html). Otherwise [the default configuration](https://github.com/detekt/detekt/blob/master/detekt-core/src/main/resources/default-detekt-config.yml) is used.
`disable_default_rulesets` | [`bool`](https://docs.bazel.build/versions/master/skylark/lib/bool.html) | `False` | See [Detekt `--disable-default-rulesets` option](https://detekt.github.io/detekt/cli.html).
`fail_fast` | [`bool`](https://docs.bazel.build/versions/master/skylark/lib/bool.html) | `False` | See [Detekt `--fail-fast` option](https://detetk.github.io/detekt/cli.html).
`html_report` | [`bool`](https://docs.bazel.build/versions/master/skylark/lib/bool.html) | `False` | Enables / disables the HTML report generation. The report file name is `{target_name}_detekt_report.html`.
`parallel` | [`bool`](https://docs.bazel.build/versions/master/skylark/lib/bool.html) | `False` | See [Detekt `--parallel` option](https://detekt.github.io/detekt/cli.html).
`plugins` | [`[Label]`](https://docs.bazel.build/versions/master/skylark/lib/list.html) | `[]` | [Detekt plugins](https://detekt.github.io/detekt/extensions.html). For example, [the formatting rule set](https://detekt.github.io/detekt/formatting.html). Labels should be JVM artifacts (generated via [`rules_jvm_external`](https://github.com/bazelbuild/rules_jvm_external) work).
`srcs` | [`[Label]`](https://docs.bazel.build/versions/master/skylark/lib/list.html) | — | Kotlin source code files.
`xml_report` | [`bool`](https://docs.bazel.build/versions/master/skylark/lib/bool.html) | `False` | Enables / disables the XML report generation. The report file name is `{target_name}_detekt_report.xml`. FYI Detekt uses the Checkstyle XML reporting format which makes it compatible with tools like SonarQube.