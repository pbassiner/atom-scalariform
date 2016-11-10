# atom-scalariform package

Allows formatting of scala files using scalariform. It also supports [Ammonite](https://github.com/lihaoyi/Ammonite) scripts.

You can configure the properties file to be used in your atom config:
```
scalariform:
  propertiesFile: "/path/to/scalariform.properties"
  relativeToProject: false
```

If `relativeToProject` is set to `true` it means the `propertiesFile` path is relative to the about-to-format file's project folder.

To format a .scala/.sc file, first save it then you can run the formatter by pressing:

```
ctrl-shift-s
```

Currently using scalariform 0.1.5 SNAPSHOT
