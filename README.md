# atom-scalariform package

Allows formatting of [Scala](https://github.com/scala/scala) files using [scalariform](https://github.com/scala-ide/scalariform). It also supports [Ammonite](https://github.com/lihaoyi/Ammonite) scripts.

You can configure the `scalariform` properties file to be used in your Atom config as an absolute or a relative path.

## Absolute properties file path
If `relativeToProject` is set to `false`, the `propertiesFile` path is considered absolute:
```
scalariform:
  propertiesFile: "/path/to/scalariform.properties"
  relativeToProject: false
```

## Relative properties file path
If `relativeToProject` is set to `true`, the `propertiesFile` path is considered relative to the about-to-format file's project folder:
```
scalariform:
  propertiesFile: "scalariform.properties"
  relativeToProject: true
```

Assuming the file to format is located at `/home/user/myProjects/myProject/src/main/scala/com/user/Test.scala` and the Atom project folder is `myProject`, the `scalariform` properties file will be loaded from `/home/user/myProjects/myProject/scalariform.properties`.

If a project folder cannot be found, the plugin will try to load the `propertiesFile` as an absolute path.

## Usage
To format a .scala/.sc file, first save it then you can run the formatter by pressing:

```
ctrl-shift-s
```

Currently using scalariform 0.1.5 SNAPSHOT
