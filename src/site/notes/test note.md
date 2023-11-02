```dataview
> > LIST
> > WHERE file.mday >= date(today-10) AND dg-publish = true AND file.name != this.file.name AND hide != true
> > SORT file.ctime asc
> > ```