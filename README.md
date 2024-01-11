# Eclipse Repackager


## Structure - for multi user / linux system installation

```
/usr/lib64/
 └ eclipse/
   ├ eclipse-platform/
   │ ├ dropins/
   │ ├ features/
   │ │ # "features" folder from:
   │ │ #   eclipse-platform-4.30-linux-gtk-x86_64.tar.gz
   │ │ #   eclipse-jee-2023-12-R-linux-gtk-x86_64.tar.gz
   │ ├ plugins/
   │ │ # "plugins" folder from:
   │ │ #   eclipse-platform-4.30-linux-gtk-x86_64.tar.gz
   │ │ #   eclipse-jee-2023-12-R-linux-gtk-x86_64.tar.gz
   │ └ eclipse_v4-30-0
   │   # "eclipse" binary from
   │   #   eclipse-platform-4.30-linux-gtk-x86_64.tar.gz
   │
   ├ eclipse-platform_v4-30-0/
   │ │ # from eclipse-platform-4.30-linux-gtk-x86_64.tar.gz
   │ ├ artifacts.xml
   │ ├ configuration
   │ │ ├ config.ini
   │ │ │ # contains modifications
   │ │ ├ org.eclipse.equinox.simpleconfigurator
   │ │ │ └ bundles.info
   │ │ └ org.eclipse.update
   │ │   └ platform.xml
   │ ├ eclipse.ini
   │ │ # contains modifications
   │ ├ icon.xpm
   │ ├ org.eclipse.epp.platform.product-2023-12.desktop
   │ │ # specially created
   │ └ readme
   │   └ readme_eclipse.html
   │
   └ eclipse-jee_v4-30-0/
     │ # from eclipse-jee-2023-12-R-linux-gtk-x86_64.tar.gz
     ├ artifacts.xml
     ├ configuration
     │ ├ config.ini
     │ │ # contains modifications
     │ ├ org.eclipse.equinox.simpleconfigurator
     │ │ └ bundles.info
     │ └ org.eclipse.update
     │   └ platform.xml
     ├ eclipse.ini
     │ # contains modifications
     ├ icon.xpm
     ├ org.eclipse.epp.package.jee.product-2023-12.desktop
     │ # specially created
     └ readme
       └ readme_eclipse.html

/usr/share/p2/
 # new home of the p2 folder - as per fedora specification
 # since "/usr/share/" is for arbitrary data, all users need but the system/users only update once 
```

## Notes


