# Snapshots from https://remlapmot.r-universe.dev

This is based on <https://github.com/jeroen/backup> but saves each snapshot into a directory named for the date, as per the MRAN and [P3M](https://p3m.dev/client/#/) snapshot repositories.

To install a package from a snapshot say from 2024-04-18 run the following code:

Windows and Mac users (assumes a P3M snapshot exists on this date - see whether <https://p3m.dev/cran/2024-04-18/src/contrib/PACKAGES> exists)

```r
install.packages('knitexercise',
  repos = c('https://remlapmot.github.io/snapshot/2024-04-18',
            'https://p3m.dev/cran/2024-04-18'))
```

Ubuntu Jammy Jellyfish users (assumes a P3M snapshot exists on this date - see whether <https://p3m.dev/cran/__linux__/jammy/2024-04-18/src/contrib/PACKAGES> exists)

```r
install.packages('knitexercise',
  repos = 'https://remlapmot.github.io/snapshot/2024-04-18/bin/linux/jammy/4.3',
          'https://p3m.dev/cran/__linux__/jammy/2024-04-18')
```

WebR users

```r
install.packages('knitexercise',
  repos = c('https://remlapmot.github.io/snapshot/2024-04-18', 'https://repo.r-wasm.org'))
```
