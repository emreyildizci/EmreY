```dataview
> > LIST rows.original_url
> > FROM "Omnivore"
> > WHERE file.mday >= (date(today) - dur(10 days)) AND dg-publish = true AND is_read = true AND hide != true
> > SORT file.mtime desc
> > GROUP BY file.cday
> > ```