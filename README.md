# api documentation for  [ramda (v0.23.0)](http://ramdajs.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-ramda.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ramda) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ramda.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ramda)
#### A practical functional library for JavaScript programmers.

[![NPM](https://nodei.co/npm/ramda.png?downloads=true)](https://www.npmjs.com/package/ramda)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ramda/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-ramda_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ramda/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-ramda/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Scott Sauyet",
        "email": "scott@sauyet.com",
        "url": "scott.sauyet.com"
    },
    "bugs": {
        "url": "https://github.com/ramda/ramda/issues"
    },
    "contributors": [
        {
            "name": "Michael Hurley",
            "email": "mh@buzzdecafe.com",
            "url": "http://buzzdecafe.com"
        },
        {
            "name": "Scott Sauyet",
            "email": "scott@sauyet.com",
            "url": "http://fr.umio.us"
        },
        {
            "name": "David Chambers",
            "email": "dc@davidchambers.me",
            "url": "http://davidchambers.me"
        },
        {
            "name": "Graeme Yeates",
            "email": "yeatesgraeme@gmail.com",
            "url": "https://github.com/megawac"
        }
    ],
    "dependencies": {},
    "description": "A practical functional library for JavaScript programmers.",
    "devDependencies": {
        "acorn": "0.9.x",
        "benchmark": "~1.0.0",
        "browserify": "10.x.x",
        "cli-table": "0.3.x",
        "commander": "2.5.x",
        "dox": "latest",
        "envvar": "1.x.x",
        "escodegen": "1.4.x",
        "eslint": "^2.11.0",
        "handlebars": "3.0.x",
        "istanbul": "^0.4.x",
        "js-yaml": "^3.2.5",
        "jsverify": "^0.7.3",
        "mocha": "2.x.x",
        "q": "^1.1.1",
        "ramda": "0.17.x",
        "rimraf": "~2.3.2",
        "sanctuary": "0.7.x",
        "sinon": "^1.17.4",
        "testem": "0.9.x",
        "uglify-js": "2.4.x",
        "xyz": "1.0.x"
    },
    "directories": {},
    "dist": {
        "shasum": "ccd13fff73497a93974e3e86327bfd87bd6e8e2b",
        "tarball": "https://registry.npmjs.org/ramda/-/ramda-0.23.0.tgz"
    },
    "gitHead": "5dec606e0504af973cd6e0ceec8997b72800eb6b",
    "homepage": "http://ramdajs.com/",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "aromano",
            "email": "aromano@preemptsecurity.com"
        },
        {
            "name": "buzzdecafe",
            "email": "m_hur@yahoo.com"
        },
        {
            "name": "crosseye",
            "email": "scott@sauyet.com"
        },
        {
            "name": "davidchambers",
            "email": "dc@davidchambers.me"
        },
        {
            "name": "kedashoe",
            "email": "kwallace@gmail.com"
        },
        {
            "name": "rane",
            "email": "raine.virta@gmail.com"
        },
        {
            "name": "scott-christopher",
            "email": "schristopher@konputa.com"
        }
    ],
    "name": "ramda",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/ramda/ramda.git"
    },
    "scripts": {
        "bench": "scripts/benchRunner",
        "bookmarklet": "scripts/bookmarklet",
        "browser_test": "testem ci",
        "build": "make && make dist/ramda.min.js",
        "clean": "rimraf dist/* coverage/*",
        "coverage": "istanbul cover node_modules/.bin/_mocha -- --reporter spec",
        "lint": "eslint scripts/bookmarklet scripts/build src/*.js src/internal/*.js test/*.js test/**/*.js lib/sauce/*.js lib/bench/*.js",
        "postbrowser_test": "npm run posttest",
        "postcoverage": "npm run posttest",
        "posttest": "git checkout -- dist",
        "prebrowser_test": "npm run pretest",
        "precoverage": "npm run pretest",
        "test": "mocha --reporter spec"
    },
    "version": "0.23.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module ramda](#apidoc.module.ramda)
1.  [function <span class="apidocSignatureSpan">ramda.</span>F ()](#apidoc.element.ramda.F)
1.  [function <span class="apidocSignatureSpan">ramda.</span>T ()](#apidoc.element.ramda.T)
1.  [function <span class="apidocSignatureSpan">ramda.</span>add (a, b)](#apidoc.element.ramda.add)
1.  [function <span class="apidocSignatureSpan">ramda.</span>addIndex (a)](#apidoc.element.ramda.addIndex)
1.  [function <span class="apidocSignatureSpan">ramda.</span>adjust (a, b, c)](#apidoc.element.ramda.adjust)
1.  [function <span class="apidocSignatureSpan">ramda.</span>all (a, b)](#apidoc.element.ramda.all)
1.  [function <span class="apidocSignatureSpan">ramda.</span>allPass (a)](#apidoc.element.ramda.allPass)
1.  [function <span class="apidocSignatureSpan">ramda.</span>always (a)](#apidoc.element.ramda.always)
1.  [function <span class="apidocSignatureSpan">ramda.</span>and (a, b)](#apidoc.element.ramda.and)
1.  [function <span class="apidocSignatureSpan">ramda.</span>any (a, b)](#apidoc.element.ramda.any)
1.  [function <span class="apidocSignatureSpan">ramda.</span>anyPass (a)](#apidoc.element.ramda.anyPass)
1.  [function <span class="apidocSignatureSpan">ramda.</span>ap (a, b)](#apidoc.element.ramda.ap)
1.  [function <span class="apidocSignatureSpan">ramda.</span>aperture (a, b)](#apidoc.element.ramda.aperture)
1.  [function <span class="apidocSignatureSpan">ramda.</span>append (a, b)](#apidoc.element.ramda.append)
1.  [function <span class="apidocSignatureSpan">ramda.</span>apply (a, b)](#apidoc.element.ramda.apply)
1.  [function <span class="apidocSignatureSpan">ramda.</span>applySpec (a)](#apidoc.element.ramda.applySpec)
1.  [function <span class="apidocSignatureSpan">ramda.</span>ascend (a, b, c)](#apidoc.element.ramda.ascend)
1.  [function <span class="apidocSignatureSpan">ramda.</span>assoc (a, b, c)](#apidoc.element.ramda.assoc)
1.  [function <span class="apidocSignatureSpan">ramda.</span>assocPath (a, b, c)](#apidoc.element.ramda.assocPath)
1.  [function <span class="apidocSignatureSpan">ramda.</span>binary (a)](#apidoc.element.ramda.binary)
1.  [function <span class="apidocSignatureSpan">ramda.</span>bind (a, b)](#apidoc.element.ramda.bind)
1.  [function <span class="apidocSignatureSpan">ramda.</span>both (a, b)](#apidoc.element.ramda.both)
1.  [function <span class="apidocSignatureSpan">ramda.</span>call (a)](#apidoc.element.ramda.call)
1.  [function <span class="apidocSignatureSpan">ramda.</span>chain (a, b)](#apidoc.element.ramda.chain)
1.  [function <span class="apidocSignatureSpan">ramda.</span>clamp (a, b, c)](#apidoc.element.ramda.clamp)
1.  [function <span class="apidocSignatureSpan">ramda.</span>clone (a)](#apidoc.element.ramda.clone)
1.  [function <span class="apidocSignatureSpan">ramda.</span>comparator (a)](#apidoc.element.ramda.comparator)
1.  [function <span class="apidocSignatureSpan">ramda.</span>complement (a)](#apidoc.element.ramda.complement)
1.  [function <span class="apidocSignatureSpan">ramda.</span>compose ()](#apidoc.element.ramda.compose)
1.  [function <span class="apidocSignatureSpan">ramda.</span>composeK ()](#apidoc.element.ramda.composeK)
1.  [function <span class="apidocSignatureSpan">ramda.</span>composeP ()](#apidoc.element.ramda.composeP)
1.  [function <span class="apidocSignatureSpan">ramda.</span>concat (a, b)](#apidoc.element.ramda.concat)
1.  [function <span class="apidocSignatureSpan">ramda.</span>cond (a)](#apidoc.element.ramda.cond)
1.  [function <span class="apidocSignatureSpan">ramda.</span>construct (a)](#apidoc.element.ramda.construct)
1.  [function <span class="apidocSignatureSpan">ramda.</span>constructN (a, b)](#apidoc.element.ramda.constructN)
1.  [function <span class="apidocSignatureSpan">ramda.</span>contains (a, b)](#apidoc.element.ramda.contains)
1.  [function <span class="apidocSignatureSpan">ramda.</span>converge (a, b)](#apidoc.element.ramda.converge)
1.  [function <span class="apidocSignatureSpan">ramda.</span>countBy (a0, a1)](#apidoc.element.ramda.countBy)
1.  [function <span class="apidocSignatureSpan">ramda.</span>curry (a)](#apidoc.element.ramda.curry)
1.  [function <span class="apidocSignatureSpan">ramda.</span>curryN (a, b)](#apidoc.element.ramda.curryN)
1.  [function <span class="apidocSignatureSpan">ramda.</span>dec (a)](#apidoc.element.ramda.dec)
1.  [function <span class="apidocSignatureSpan">ramda.</span>defaultTo (a, b)](#apidoc.element.ramda.defaultTo)
1.  [function <span class="apidocSignatureSpan">ramda.</span>descend (a, b, c)](#apidoc.element.ramda.descend)
1.  [function <span class="apidocSignatureSpan">ramda.</span>difference (a, b)](#apidoc.element.ramda.difference)
1.  [function <span class="apidocSignatureSpan">ramda.</span>differenceWith (a, b, c)](#apidoc.element.ramda.differenceWith)
1.  [function <span class="apidocSignatureSpan">ramda.</span>dissoc (a, b)](#apidoc.element.ramda.dissoc)
1.  [function <span class="apidocSignatureSpan">ramda.</span>dissocPath (a, b)](#apidoc.element.ramda.dissocPath)
1.  [function <span class="apidocSignatureSpan">ramda.</span>divide (a, b)](#apidoc.element.ramda.divide)
1.  [function <span class="apidocSignatureSpan">ramda.</span>drop (a, b)](#apidoc.element.ramda.drop)
1.  [function <span class="apidocSignatureSpan">ramda.</span>dropLast (a, b)](#apidoc.element.ramda.dropLast)
1.  [function <span class="apidocSignatureSpan">ramda.</span>dropLastWhile (a, b)](#apidoc.element.ramda.dropLastWhile)
1.  [function <span class="apidocSignatureSpan">ramda.</span>dropRepeats (a)](#apidoc.element.ramda.dropRepeats)
1.  [function <span class="apidocSignatureSpan">ramda.</span>dropRepeatsWith (a, b)](#apidoc.element.ramda.dropRepeatsWith)
1.  [function <span class="apidocSignatureSpan">ramda.</span>dropWhile (a, b)](#apidoc.element.ramda.dropWhile)
1.  [function <span class="apidocSignatureSpan">ramda.</span>either (a, b)](#apidoc.element.ramda.either)
1.  [function <span class="apidocSignatureSpan">ramda.</span>empty (a)](#apidoc.element.ramda.empty)
1.  [function <span class="apidocSignatureSpan">ramda.</span>eqBy (a, b, c)](#apidoc.element.ramda.eqBy)
1.  [function <span class="apidocSignatureSpan">ramda.</span>eqProps (a, b, c)](#apidoc.element.ramda.eqProps)
1.  [function <span class="apidocSignatureSpan">ramda.</span>equals (a, b)](#apidoc.element.ramda.equals)
1.  [function <span class="apidocSignatureSpan">ramda.</span>evolve (a, b)](#apidoc.element.ramda.evolve)
1.  [function <span class="apidocSignatureSpan">ramda.</span>filter (a, b)](#apidoc.element.ramda.filter)
1.  [function <span class="apidocSignatureSpan">ramda.</span>find (a, b)](#apidoc.element.ramda.find)
1.  [function <span class="apidocSignatureSpan">ramda.</span>findIndex (a, b)](#apidoc.element.ramda.findIndex)
1.  [function <span class="apidocSignatureSpan">ramda.</span>findLast (a, b)](#apidoc.element.ramda.findLast)
1.  [function <span class="apidocSignatureSpan">ramda.</span>findLastIndex (a, b)](#apidoc.element.ramda.findLastIndex)
1.  [function <span class="apidocSignatureSpan">ramda.</span>flatten (a)](#apidoc.element.ramda.flatten)
1.  [function <span class="apidocSignatureSpan">ramda.</span>flip (a)](#apidoc.element.ramda.flip)
1.  [function <span class="apidocSignatureSpan">ramda.</span>forEach (a, b)](#apidoc.element.ramda.forEach)
1.  [function <span class="apidocSignatureSpan">ramda.</span>forEachObjIndexed (a, b)](#apidoc.element.ramda.forEachObjIndexed)
1.  [function <span class="apidocSignatureSpan">ramda.</span>fromPairs (a)](#apidoc.element.ramda.fromPairs)
1.  [function <span class="apidocSignatureSpan">ramda.</span>groupBy (a, b)](#apidoc.element.ramda.groupBy)
1.  [function <span class="apidocSignatureSpan">ramda.</span>groupWith (a, b)](#apidoc.element.ramda.groupWith)
1.  [function <span class="apidocSignatureSpan">ramda.</span>gt (a, b)](#apidoc.element.ramda.gt)
1.  [function <span class="apidocSignatureSpan">ramda.</span>gte (a, b)](#apidoc.element.ramda.gte)
1.  [function <span class="apidocSignatureSpan">ramda.</span>has (a, b)](#apidoc.element.ramda.has)
1.  [function <span class="apidocSignatureSpan">ramda.</span>hasIn (a, b)](#apidoc.element.ramda.hasIn)
1.  [function <span class="apidocSignatureSpan">ramda.</span>head (a)](#apidoc.element.ramda.head)
1.  [function <span class="apidocSignatureSpan">ramda.</span>identical (a, b)](#apidoc.element.ramda.identical)
1.  [function <span class="apidocSignatureSpan">ramda.</span>identity (a)](#apidoc.element.ramda.identity)
1.  [function <span class="apidocSignatureSpan">ramda.</span>ifElse (a, b, c)](#apidoc.element.ramda.ifElse)
1.  [function <span class="apidocSignatureSpan">ramda.</span>inc (a)](#apidoc.element.ramda.inc)
1.  [function <span class="apidocSignatureSpan">ramda.</span>indexBy (a0, a1)](#apidoc.element.ramda.indexBy)
1.  [function <span class="apidocSignatureSpan">ramda.</span>indexOf (a, b)](#apidoc.element.ramda.indexOf)
1.  [function <span class="apidocSignatureSpan">ramda.</span>init (a)](#apidoc.element.ramda.init)
1.  [function <span class="apidocSignatureSpan">ramda.</span>insert (a, b, c)](#apidoc.element.ramda.insert)
1.  [function <span class="apidocSignatureSpan">ramda.</span>insertAll (a, b, c)](#apidoc.element.ramda.insertAll)
1.  [function <span class="apidocSignatureSpan">ramda.</span>intersection (a, b)](#apidoc.element.ramda.intersection)
1.  [function <span class="apidocSignatureSpan">ramda.</span>intersectionWith (a, b, c)](#apidoc.element.ramda.intersectionWith)
1.  [function <span class="apidocSignatureSpan">ramda.</span>intersperse (a, b)](#apidoc.element.ramda.intersperse)
1.  [function <span class="apidocSignatureSpan">ramda.</span>into (a, b, c)](#apidoc.element.ramda.into)
1.  [function <span class="apidocSignatureSpan">ramda.</span>invert (a)](#apidoc.element.ramda.invert)
1.  [function <span class="apidocSignatureSpan">ramda.</span>invertObj (a)](#apidoc.element.ramda.invertObj)
1.  [function <span class="apidocSignatureSpan">ramda.</span>invoker (a, b)](#apidoc.element.ramda.invoker)
1.  [function <span class="apidocSignatureSpan">ramda.</span>is (a, b)](#apidoc.element.ramda.is)
1.  [function <span class="apidocSignatureSpan">ramda.</span>isArrayLike (a)](#apidoc.element.ramda.isArrayLike)
1.  [function <span class="apidocSignatureSpan">ramda.</span>isEmpty (a)](#apidoc.element.ramda.isEmpty)
1.  [function <span class="apidocSignatureSpan">ramda.</span>isNil (a)](#apidoc.element.ramda.isNil)
1.  [function <span class="apidocSignatureSpan">ramda.</span>join (a0, a1)](#apidoc.element.ramda.join)
1.  [function <span class="apidocSignatureSpan">ramda.</span>juxt (a)](#apidoc.element.ramda.juxt)
1.  [function <span class="apidocSignatureSpan">ramda.</span>keys (a)](#apidoc.element.ramda.keys)
1.  [function <span class="apidocSignatureSpan">ramda.</span>keysIn (a)](#apidoc.element.ramda.keysIn)
1.  [function <span class="apidocSignatureSpan">ramda.</span>last (a)](#apidoc.element.ramda.last)
1.  [function <span class="apidocSignatureSpan">ramda.</span>lastIndexOf (a, b)](#apidoc.element.ramda.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">ramda.</span>length (a)](#apidoc.element.ramda.length)
1.  [function <span class="apidocSignatureSpan">ramda.</span>lens (a, b)](#apidoc.element.ramda.lens)
1.  [function <span class="apidocSignatureSpan">ramda.</span>lensIndex (a)](#apidoc.element.ramda.lensIndex)
1.  [function <span class="apidocSignatureSpan">ramda.</span>lensPath (a)](#apidoc.element.ramda.lensPath)
1.  [function <span class="apidocSignatureSpan">ramda.</span>lensProp (a)](#apidoc.element.ramda.lensProp)
1.  [function <span class="apidocSignatureSpan">ramda.</span>lift (a)](#apidoc.element.ramda.lift)
1.  [function <span class="apidocSignatureSpan">ramda.</span>liftN (a, b)](#apidoc.element.ramda.liftN)
1.  [function <span class="apidocSignatureSpan">ramda.</span>lt (a, b)](#apidoc.element.ramda.lt)
1.  [function <span class="apidocSignatureSpan">ramda.</span>lte (a, b)](#apidoc.element.ramda.lte)
1.  [function <span class="apidocSignatureSpan">ramda.</span>map (a, b)](#apidoc.element.ramda.map)
1.  [function <span class="apidocSignatureSpan">ramda.</span>mapAccum (a, b, c)](#apidoc.element.ramda.mapAccum)
1.  [function <span class="apidocSignatureSpan">ramda.</span>mapAccumRight (a, b, c)](#apidoc.element.ramda.mapAccumRight)
1.  [function <span class="apidocSignatureSpan">ramda.</span>mapObjIndexed (a, b)](#apidoc.element.ramda.mapObjIndexed)
1.  [function <span class="apidocSignatureSpan">ramda.</span>match (a, b)](#apidoc.element.ramda.match)
1.  [function <span class="apidocSignatureSpan">ramda.</span>mathMod (a, b)](#apidoc.element.ramda.mathMod)
1.  [function <span class="apidocSignatureSpan">ramda.</span>max (a, b)](#apidoc.element.ramda.max)
1.  [function <span class="apidocSignatureSpan">ramda.</span>maxBy (a, b, c)](#apidoc.element.ramda.maxBy)
1.  [function <span class="apidocSignatureSpan">ramda.</span>mean (a)](#apidoc.element.ramda.mean)
1.  [function <span class="apidocSignatureSpan">ramda.</span>median (a)](#apidoc.element.ramda.median)
1.  [function <span class="apidocSignatureSpan">ramda.</span>memoize (a)](#apidoc.element.ramda.memoize)
1.  [function <span class="apidocSignatureSpan">ramda.</span>merge (a, b)](#apidoc.element.ramda.merge)
1.  [function <span class="apidocSignatureSpan">ramda.</span>mergeAll (a)](#apidoc.element.ramda.mergeAll)
1.  [function <span class="apidocSignatureSpan">ramda.</span>mergeWith (a, b, c)](#apidoc.element.ramda.mergeWith)
1.  [function <span class="apidocSignatureSpan">ramda.</span>mergeWithKey (a, b, c)](#apidoc.element.ramda.mergeWithKey)
1.  [function <span class="apidocSignatureSpan">ramda.</span>min (a, b)](#apidoc.element.ramda.min)
1.  [function <span class="apidocSignatureSpan">ramda.</span>minBy (a, b, c)](#apidoc.element.ramda.minBy)
1.  [function <span class="apidocSignatureSpan">ramda.</span>modulo (a, b)](#apidoc.element.ramda.modulo)
1.  [function <span class="apidocSignatureSpan">ramda.</span>multiply (a, b)](#apidoc.element.ramda.multiply)
1.  [function <span class="apidocSignatureSpan">ramda.</span>nAry (a, b)](#apidoc.element.ramda.nAry)
1.  [function <span class="apidocSignatureSpan">ramda.</span>negate (a)](#apidoc.element.ramda.negate)
1.  [function <span class="apidocSignatureSpan">ramda.</span>none (a, b)](#apidoc.element.ramda.none)
1.  [function <span class="apidocSignatureSpan">ramda.</span>not (a)](#apidoc.element.ramda.not)
1.  [function <span class="apidocSignatureSpan">ramda.</span>nth (a, b)](#apidoc.element.ramda.nth)
1.  [function <span class="apidocSignatureSpan">ramda.</span>nthArg (a)](#apidoc.element.ramda.nthArg)
1.  [function <span class="apidocSignatureSpan">ramda.</span>objOf (a, b)](#apidoc.element.ramda.objOf)
1.  [function <span class="apidocSignatureSpan">ramda.</span>of (a)](#apidoc.element.ramda.of)
1.  [function <span class="apidocSignatureSpan">ramda.</span>omit (a, b)](#apidoc.element.ramda.omit)
1.  [function <span class="apidocSignatureSpan">ramda.</span>once (a)](#apidoc.element.ramda.once)
1.  [function <span class="apidocSignatureSpan">ramda.</span>or (a, b)](#apidoc.element.ramda.or)
1.  [function <span class="apidocSignatureSpan">ramda.</span>over (a, b, c)](#apidoc.element.ramda.over)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pair (a, b)](#apidoc.element.ramda.pair)
1.  [function <span class="apidocSignatureSpan">ramda.</span>partial (a, b)](#apidoc.element.ramda.partial)
1.  [function <span class="apidocSignatureSpan">ramda.</span>partialRight (a, b)](#apidoc.element.ramda.partialRight)
1.  [function <span class="apidocSignatureSpan">ramda.</span>partition (a0, a1)](#apidoc.element.ramda.partition)
1.  [function <span class="apidocSignatureSpan">ramda.</span>path (a, b)](#apidoc.element.ramda.path)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pathEq (a, b, c)](#apidoc.element.ramda.pathEq)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pathOr (a, b, c)](#apidoc.element.ramda.pathOr)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pathSatisfies (a, b, c)](#apidoc.element.ramda.pathSatisfies)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pick (a, b)](#apidoc.element.ramda.pick)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pickAll (a, b)](#apidoc.element.ramda.pickAll)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pickBy (a, b)](#apidoc.element.ramda.pickBy)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pipe ()](#apidoc.element.ramda.pipe)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pipeK ()](#apidoc.element.ramda.pipeK)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pipeP ()](#apidoc.element.ramda.pipeP)
1.  [function <span class="apidocSignatureSpan">ramda.</span>pluck (a, b)](#apidoc.element.ramda.pluck)
1.  [function <span class="apidocSignatureSpan">ramda.</span>prepend (a, b)](#apidoc.element.ramda.prepend)
1.  [function <span class="apidocSignatureSpan">ramda.</span>product (a)](#apidoc.element.ramda.product)
1.  [function <span class="apidocSignatureSpan">ramda.</span>project (a0, a1)](#apidoc.element.ramda.project)
1.  [function <span class="apidocSignatureSpan">ramda.</span>prop (a, b)](#apidoc.element.ramda.prop)
1.  [function <span class="apidocSignatureSpan">ramda.</span>propEq (a, b, c)](#apidoc.element.ramda.propEq)
1.  [function <span class="apidocSignatureSpan">ramda.</span>propIs (a, b, c)](#apidoc.element.ramda.propIs)
1.  [function <span class="apidocSignatureSpan">ramda.</span>propOr (a, b, c)](#apidoc.element.ramda.propOr)
1.  [function <span class="apidocSignatureSpan">ramda.</span>propSatisfies (a, b, c)](#apidoc.element.ramda.propSatisfies)
1.  [function <span class="apidocSignatureSpan">ramda.</span>props (a, b)](#apidoc.element.ramda.props)
1.  [function <span class="apidocSignatureSpan">ramda.</span>range (a, b)](#apidoc.element.ramda.range)
1.  [function <span class="apidocSignatureSpan">ramda.</span>reduce (a, b, c)](#apidoc.element.ramda.reduce)
1.  [function <span class="apidocSignatureSpan">ramda.</span>reduceBy ()](#apidoc.element.ramda.reduceBy)
1.  [function <span class="apidocSignatureSpan">ramda.</span>reduceRight (a, b, c)](#apidoc.element.ramda.reduceRight)
1.  [function <span class="apidocSignatureSpan">ramda.</span>reduceWhile ()](#apidoc.element.ramda.reduceWhile)
1.  [function <span class="apidocSignatureSpan">ramda.</span>reduced (a)](#apidoc.element.ramda.reduced)
1.  [function <span class="apidocSignatureSpan">ramda.</span>reject (a, b)](#apidoc.element.ramda.reject)
1.  [function <span class="apidocSignatureSpan">ramda.</span>remove (a, b, c)](#apidoc.element.ramda.remove)
1.  [function <span class="apidocSignatureSpan">ramda.</span>repeat (a, b)](#apidoc.element.ramda.repeat)
1.  [function <span class="apidocSignatureSpan">ramda.</span>replace (a, b, c)](#apidoc.element.ramda.replace)
1.  [function <span class="apidocSignatureSpan">ramda.</span>reverse (a)](#apidoc.element.ramda.reverse)
1.  [function <span class="apidocSignatureSpan">ramda.</span>scan (a, b, c)](#apidoc.element.ramda.scan)
1.  [function <span class="apidocSignatureSpan">ramda.</span>sequence (a, b)](#apidoc.element.ramda.sequence)
1.  [function <span class="apidocSignatureSpan">ramda.</span>set (a, b, c)](#apidoc.element.ramda.set)
1.  [function <span class="apidocSignatureSpan">ramda.</span>slice (a, b, c)](#apidoc.element.ramda.slice)
1.  [function <span class="apidocSignatureSpan">ramda.</span>sort (a, b)](#apidoc.element.ramda.sort)
1.  [function <span class="apidocSignatureSpan">ramda.</span>sortBy (a, b)](#apidoc.element.ramda.sortBy)
1.  [function <span class="apidocSignatureSpan">ramda.</span>sortWith (a, b)](#apidoc.element.ramda.sortWith)
1.  [function <span class="apidocSignatureSpan">ramda.</span>split (a0, a1)](#apidoc.element.ramda.split)
1.  [function <span class="apidocSignatureSpan">ramda.</span>splitAt (a, b)](#apidoc.element.ramda.splitAt)
1.  [function <span class="apidocSignatureSpan">ramda.</span>splitEvery (a, b)](#apidoc.element.ramda.splitEvery)
1.  [function <span class="apidocSignatureSpan">ramda.</span>splitWhen (a, b)](#apidoc.element.ramda.splitWhen)
1.  [function <span class="apidocSignatureSpan">ramda.</span>subtract (a, b)](#apidoc.element.ramda.subtract)
1.  [function <span class="apidocSignatureSpan">ramda.</span>sum (a)](#apidoc.element.ramda.sum)
1.  [function <span class="apidocSignatureSpan">ramda.</span>symmetricDifference (a, b)](#apidoc.element.ramda.symmetricDifference)
1.  [function <span class="apidocSignatureSpan">ramda.</span>symmetricDifferenceWith (a, b, c)](#apidoc.element.ramda.symmetricDifferenceWith)
1.  [function <span class="apidocSignatureSpan">ramda.</span>tail (a)](#apidoc.element.ramda.tail)
1.  [function <span class="apidocSignatureSpan">ramda.</span>take (a, b)](#apidoc.element.ramda.take)
1.  [function <span class="apidocSignatureSpan">ramda.</span>takeLast (a, b)](#apidoc.element.ramda.takeLast)
1.  [function <span class="apidocSignatureSpan">ramda.</span>takeLastWhile (a, b)](#apidoc.element.ramda.takeLastWhile)
1.  [function <span class="apidocSignatureSpan">ramda.</span>takeWhile (a, b)](#apidoc.element.ramda.takeWhile)
1.  [function <span class="apidocSignatureSpan">ramda.</span>tap (a, b)](#apidoc.element.ramda.tap)
1.  [function <span class="apidocSignatureSpan">ramda.</span>test (a, b)](#apidoc.element.ramda.test)
1.  [function <span class="apidocSignatureSpan">ramda.</span>times (a, b)](#apidoc.element.ramda.times)
1.  [function <span class="apidocSignatureSpan">ramda.</span>toLower (a)](#apidoc.element.ramda.toLower)
1.  [function <span class="apidocSignatureSpan">ramda.</span>toPairs (a)](#apidoc.element.ramda.toPairs)
1.  [function <span class="apidocSignatureSpan">ramda.</span>toPairsIn (a)](#apidoc.element.ramda.toPairsIn)
1.  [function <span class="apidocSignatureSpan">ramda.</span>toUpper (a)](#apidoc.element.ramda.toUpper)
1.  [function <span class="apidocSignatureSpan">ramda.</span>transduce (a0, a1, a2, a3)](#apidoc.element.ramda.transduce)
1.  [function <span class="apidocSignatureSpan">ramda.</span>transpose (a)](#apidoc.element.ramda.transpose)
1.  [function <span class="apidocSignatureSpan">ramda.</span>traverse (a, b, c)](#apidoc.element.ramda.traverse)
1.  [function <span class="apidocSignatureSpan">ramda.</span>trim (a)](#apidoc.element.ramda.trim)
1.  [function <span class="apidocSignatureSpan">ramda.</span>tryCatch (a, b)](#apidoc.element.ramda.tryCatch)
1.  [function <span class="apidocSignatureSpan">ramda.</span>type (a)](#apidoc.element.ramda.type)
1.  [function <span class="apidocSignatureSpan">ramda.</span>unapply (a)](#apidoc.element.ramda.unapply)
1.  [function <span class="apidocSignatureSpan">ramda.</span>unary (a)](#apidoc.element.ramda.unary)
1.  [function <span class="apidocSignatureSpan">ramda.</span>uncurryN (a, b)](#apidoc.element.ramda.uncurryN)
1.  [function <span class="apidocSignatureSpan">ramda.</span>unfold (a, b)](#apidoc.element.ramda.unfold)
1.  [function <span class="apidocSignatureSpan">ramda.</span>union (a, b)](#apidoc.element.ramda.union)
1.  [function <span class="apidocSignatureSpan">ramda.</span>unionWith (a, b, c)](#apidoc.element.ramda.unionWith)
1.  [function <span class="apidocSignatureSpan">ramda.</span>uniq (a)](#apidoc.element.ramda.uniq)
1.  [function <span class="apidocSignatureSpan">ramda.</span>uniqBy (a, b)](#apidoc.element.ramda.uniqBy)
1.  [function <span class="apidocSignatureSpan">ramda.</span>uniqWith (a, b)](#apidoc.element.ramda.uniqWith)
1.  [function <span class="apidocSignatureSpan">ramda.</span>unless (a, b, c)](#apidoc.element.ramda.unless)
1.  [function <span class="apidocSignatureSpan">ramda.</span>unnest (a)](#apidoc.element.ramda.unnest)
1.  [function <span class="apidocSignatureSpan">ramda.</span>until (a, b, c)](#apidoc.element.ramda.until)
1.  [function <span class="apidocSignatureSpan">ramda.</span>update (a, b, c)](#apidoc.element.ramda.update)
1.  [function <span class="apidocSignatureSpan">ramda.</span>useWith (a, b)](#apidoc.element.ramda.useWith)
1.  [function <span class="apidocSignatureSpan">ramda.</span>values (a)](#apidoc.element.ramda.values)
1.  [function <span class="apidocSignatureSpan">ramda.</span>valuesIn (a)](#apidoc.element.ramda.valuesIn)
1.  [function <span class="apidocSignatureSpan">ramda.</span>view (a, b)](#apidoc.element.ramda.view)
1.  [function <span class="apidocSignatureSpan">ramda.</span>when (a, b, c)](#apidoc.element.ramda.when)
1.  [function <span class="apidocSignatureSpan">ramda.</span>where (a, b)](#apidoc.element.ramda.where)
1.  [function <span class="apidocSignatureSpan">ramda.</span>whereEq (a, b)](#apidoc.element.ramda.whereEq)
1.  [function <span class="apidocSignatureSpan">ramda.</span>without (a, b)](#apidoc.element.ramda.without)
1.  [function <span class="apidocSignatureSpan">ramda.</span>xprod (a, b)](#apidoc.element.ramda.xprod)
1.  [function <span class="apidocSignatureSpan">ramda.</span>zip (a, b)](#apidoc.element.ramda.zip)
1.  [function <span class="apidocSignatureSpan">ramda.</span>zipObj (a, b)](#apidoc.element.ramda.zipObj)
1.  [function <span class="apidocSignatureSpan">ramda.</span>zipWith (a, b, c)](#apidoc.element.ramda.zipWith)
1.  object <span class="apidocSignatureSpan">ramda.</span>__



# <a name="apidoc.module.ramda"></a>[module ramda](#apidoc.module.ramda)

#### <a name="apidoc.element.ramda.F"></a>[function <span class="apidocSignatureSpan">ramda.</span>F ()](#apidoc.element.ramda.F)
- description and source-code
```javascript
F = function () {
  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.T"></a>[function <span class="apidocSignatureSpan">ramda.</span>T ()](#apidoc.element.ramda.T)
- description and source-code
```javascript
T = function () {
  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.add"></a>[function <span class="apidocSignatureSpan">ramda.</span>add (a, b)](#apidoc.element.ramda.add)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.addIndex"></a>[function <span class="apidocSignatureSpan">ramda.</span>addIndex (a)](#apidoc.element.ramda.addIndex)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.adjust"></a>[function <span class="apidocSignatureSpan">ramda.</span>adjust (a, b, c)](#apidoc.element.ramda.adjust)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.all"></a>[function <span class="apidocSignatureSpan">ramda.</span>all (a, b)](#apidoc.element.ramda.all)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.allPass"></a>[function <span class="apidocSignatureSpan">ramda.</span>allPass (a)](#apidoc.element.ramda.allPass)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.always"></a>[function <span class="apidocSignatureSpan">ramda.</span>always (a)](#apidoc.element.ramda.always)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.and"></a>[function <span class="apidocSignatureSpan">ramda.</span>and (a, b)](#apidoc.element.ramda.and)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.any"></a>[function <span class="apidocSignatureSpan">ramda.</span>any (a, b)](#apidoc.element.ramda.any)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.anyPass"></a>[function <span class="apidocSignatureSpan">ramda.</span>anyPass (a)](#apidoc.element.ramda.anyPass)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.ap"></a>[function <span class="apidocSignatureSpan">ramda.</span>ap (a, b)](#apidoc.element.ramda.ap)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.aperture"></a>[function <span class="apidocSignatureSpan">ramda.</span>aperture (a, b)](#apidoc.element.ramda.aperture)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.append"></a>[function <span class="apidocSignatureSpan">ramda.</span>append (a, b)](#apidoc.element.ramda.append)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.apply"></a>[function <span class="apidocSignatureSpan">ramda.</span>apply (a, b)](#apidoc.element.ramda.apply)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.applySpec"></a>[function <span class="apidocSignatureSpan">ramda.</span>applySpec (a)](#apidoc.element.ramda.applySpec)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.ascend"></a>[function <span class="apidocSignatureSpan">ramda.</span>ascend (a, b, c)](#apidoc.element.ramda.ascend)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.assoc"></a>[function <span class="apidocSignatureSpan">ramda.</span>assoc (a, b, c)](#apidoc.element.ramda.assoc)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.assocPath"></a>[function <span class="apidocSignatureSpan">ramda.</span>assocPath (a, b, c)](#apidoc.element.ramda.assocPath)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.binary"></a>[function <span class="apidocSignatureSpan">ramda.</span>binary (a)](#apidoc.element.ramda.binary)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.bind"></a>[function <span class="apidocSignatureSpan">ramda.</span>bind (a, b)](#apidoc.element.ramda.bind)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.both"></a>[function <span class="apidocSignatureSpan">ramda.</span>both (a, b)](#apidoc.element.ramda.both)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.call"></a>[function <span class="apidocSignatureSpan">ramda.</span>call (a)](#apidoc.element.ramda.call)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.chain"></a>[function <span class="apidocSignatureSpan">ramda.</span>chain (a, b)](#apidoc.element.ramda.chain)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.clamp"></a>[function <span class="apidocSignatureSpan">ramda.</span>clamp (a, b, c)](#apidoc.element.ramda.clamp)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.clone"></a>[function <span class="apidocSignatureSpan">ramda.</span>clone (a)](#apidoc.element.ramda.clone)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.comparator"></a>[function <span class="apidocSignatureSpan">ramda.</span>comparator (a)](#apidoc.element.ramda.comparator)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.complement"></a>[function <span class="apidocSignatureSpan">ramda.</span>complement (a)](#apidoc.element.ramda.complement)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.compose"></a>[function <span class="apidocSignatureSpan">ramda.</span>compose ()](#apidoc.element.ramda.compose)
- description and source-code
```javascript
function compose() {
  if (arguments.length === 0) {
    throw new Error('compose requires at least one argument');
  }
  return pipe.apply(this, reverse(arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.composeK"></a>[function <span class="apidocSignatureSpan">ramda.</span>composeK ()](#apidoc.element.ramda.composeK)
- description and source-code
```javascript
function composeK() {
  if (arguments.length === 0) {
    throw new Error('composeK requires at least one argument');
  }
  var init = Array.prototype.slice.call(arguments);
  var last = init.pop();
  return compose(compose.apply(this, map(chain, init)), last);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.composeP"></a>[function <span class="apidocSignatureSpan">ramda.</span>composeP ()](#apidoc.element.ramda.composeP)
- description and source-code
```javascript
function composeP() {
  if (arguments.length === 0) {
    throw new Error('composeP requires at least one argument');
  }
  return pipeP.apply(this, reverse(arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.concat"></a>[function <span class="apidocSignatureSpan">ramda.</span>concat (a, b)](#apidoc.element.ramda.concat)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.cond"></a>[function <span class="apidocSignatureSpan">ramda.</span>cond (a)](#apidoc.element.ramda.cond)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.construct"></a>[function <span class="apidocSignatureSpan">ramda.</span>construct (a)](#apidoc.element.ramda.construct)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.constructN"></a>[function <span class="apidocSignatureSpan">ramda.</span>constructN (a, b)](#apidoc.element.ramda.constructN)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.contains"></a>[function <span class="apidocSignatureSpan">ramda.</span>contains (a, b)](#apidoc.element.ramda.contains)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.converge"></a>[function <span class="apidocSignatureSpan">ramda.</span>converge (a, b)](#apidoc.element.ramda.converge)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.countBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>countBy (a0, a1)](#apidoc.element.ramda.countBy)
- description and source-code
```javascript
countBy = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.curry"></a>[function <span class="apidocSignatureSpan">ramda.</span>curry (a)](#apidoc.element.ramda.curry)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.curryN"></a>[function <span class="apidocSignatureSpan">ramda.</span>curryN (a, b)](#apidoc.element.ramda.curryN)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.dec"></a>[function <span class="apidocSignatureSpan">ramda.</span>dec (a)](#apidoc.element.ramda.dec)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.defaultTo"></a>[function <span class="apidocSignatureSpan">ramda.</span>defaultTo (a, b)](#apidoc.element.ramda.defaultTo)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.descend"></a>[function <span class="apidocSignatureSpan">ramda.</span>descend (a, b, c)](#apidoc.element.ramda.descend)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.difference"></a>[function <span class="apidocSignatureSpan">ramda.</span>difference (a, b)](#apidoc.element.ramda.difference)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.differenceWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>differenceWith (a, b, c)](#apidoc.element.ramda.differenceWith)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.dissoc"></a>[function <span class="apidocSignatureSpan">ramda.</span>dissoc (a, b)](#apidoc.element.ramda.dissoc)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.dissocPath"></a>[function <span class="apidocSignatureSpan">ramda.</span>dissocPath (a, b)](#apidoc.element.ramda.dissocPath)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.divide"></a>[function <span class="apidocSignatureSpan">ramda.</span>divide (a, b)](#apidoc.element.ramda.divide)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.drop"></a>[function <span class="apidocSignatureSpan">ramda.</span>drop (a, b)](#apidoc.element.ramda.drop)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.dropLast"></a>[function <span class="apidocSignatureSpan">ramda.</span>dropLast (a, b)](#apidoc.element.ramda.dropLast)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.dropLastWhile"></a>[function <span class="apidocSignatureSpan">ramda.</span>dropLastWhile (a, b)](#apidoc.element.ramda.dropLastWhile)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.dropRepeats"></a>[function <span class="apidocSignatureSpan">ramda.</span>dropRepeats (a)](#apidoc.element.ramda.dropRepeats)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.dropRepeatsWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>dropRepeatsWith (a, b)](#apidoc.element.ramda.dropRepeatsWith)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.dropWhile"></a>[function <span class="apidocSignatureSpan">ramda.</span>dropWhile (a, b)](#apidoc.element.ramda.dropWhile)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.either"></a>[function <span class="apidocSignatureSpan">ramda.</span>either (a, b)](#apidoc.element.ramda.either)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.empty"></a>[function <span class="apidocSignatureSpan">ramda.</span>empty (a)](#apidoc.element.ramda.empty)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.eqBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>eqBy (a, b, c)](#apidoc.element.ramda.eqBy)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.eqProps"></a>[function <span class="apidocSignatureSpan">ramda.</span>eqProps (a, b, c)](#apidoc.element.ramda.eqProps)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.equals"></a>[function <span class="apidocSignatureSpan">ramda.</span>equals (a, b)](#apidoc.element.ramda.equals)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.evolve"></a>[function <span class="apidocSignatureSpan">ramda.</span>evolve (a, b)](#apidoc.element.ramda.evolve)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.filter"></a>[function <span class="apidocSignatureSpan">ramda.</span>filter (a, b)](#apidoc.element.ramda.filter)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.find"></a>[function <span class="apidocSignatureSpan">ramda.</span>find (a, b)](#apidoc.element.ramda.find)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.findIndex"></a>[function <span class="apidocSignatureSpan">ramda.</span>findIndex (a, b)](#apidoc.element.ramda.findIndex)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.findLast"></a>[function <span class="apidocSignatureSpan">ramda.</span>findLast (a, b)](#apidoc.element.ramda.findLast)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.findLastIndex"></a>[function <span class="apidocSignatureSpan">ramda.</span>findLastIndex (a, b)](#apidoc.element.ramda.findLastIndex)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.flatten"></a>[function <span class="apidocSignatureSpan">ramda.</span>flatten (a)](#apidoc.element.ramda.flatten)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.flip"></a>[function <span class="apidocSignatureSpan">ramda.</span>flip (a)](#apidoc.element.ramda.flip)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.forEach"></a>[function <span class="apidocSignatureSpan">ramda.</span>forEach (a, b)](#apidoc.element.ramda.forEach)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.forEachObjIndexed"></a>[function <span class="apidocSignatureSpan">ramda.</span>forEachObjIndexed (a, b)](#apidoc.element.ramda.forEachObjIndexed)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.fromPairs"></a>[function <span class="apidocSignatureSpan">ramda.</span>fromPairs (a)](#apidoc.element.ramda.fromPairs)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.groupBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>groupBy (a, b)](#apidoc.element.ramda.groupBy)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.groupWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>groupWith (a, b)](#apidoc.element.ramda.groupWith)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.gt"></a>[function <span class="apidocSignatureSpan">ramda.</span>gt (a, b)](#apidoc.element.ramda.gt)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.gte"></a>[function <span class="apidocSignatureSpan">ramda.</span>gte (a, b)](#apidoc.element.ramda.gte)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.has"></a>[function <span class="apidocSignatureSpan">ramda.</span>has (a, b)](#apidoc.element.ramda.has)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.hasIn"></a>[function <span class="apidocSignatureSpan">ramda.</span>hasIn (a, b)](#apidoc.element.ramda.hasIn)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.head"></a>[function <span class="apidocSignatureSpan">ramda.</span>head (a)](#apidoc.element.ramda.head)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.identical"></a>[function <span class="apidocSignatureSpan">ramda.</span>identical (a, b)](#apidoc.element.ramda.identical)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.identity"></a>[function <span class="apidocSignatureSpan">ramda.</span>identity (a)](#apidoc.element.ramda.identity)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.ifElse"></a>[function <span class="apidocSignatureSpan">ramda.</span>ifElse (a, b, c)](#apidoc.element.ramda.ifElse)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.inc"></a>[function <span class="apidocSignatureSpan">ramda.</span>inc (a)](#apidoc.element.ramda.inc)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.indexBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>indexBy (a0, a1)](#apidoc.element.ramda.indexBy)
- description and source-code
```javascript
indexBy = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.indexOf"></a>[function <span class="apidocSignatureSpan">ramda.</span>indexOf (a, b)](#apidoc.element.ramda.indexOf)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.init"></a>[function <span class="apidocSignatureSpan">ramda.</span>init (a)](#apidoc.element.ramda.init)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.insert"></a>[function <span class="apidocSignatureSpan">ramda.</span>insert (a, b, c)](#apidoc.element.ramda.insert)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.insertAll"></a>[function <span class="apidocSignatureSpan">ramda.</span>insertAll (a, b, c)](#apidoc.element.ramda.insertAll)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.intersection"></a>[function <span class="apidocSignatureSpan">ramda.</span>intersection (a, b)](#apidoc.element.ramda.intersection)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.intersectionWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>intersectionWith (a, b, c)](#apidoc.element.ramda.intersectionWith)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.intersperse"></a>[function <span class="apidocSignatureSpan">ramda.</span>intersperse (a, b)](#apidoc.element.ramda.intersperse)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.into"></a>[function <span class="apidocSignatureSpan">ramda.</span>into (a, b, c)](#apidoc.element.ramda.into)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.invert"></a>[function <span class="apidocSignatureSpan">ramda.</span>invert (a)](#apidoc.element.ramda.invert)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.invertObj"></a>[function <span class="apidocSignatureSpan">ramda.</span>invertObj (a)](#apidoc.element.ramda.invertObj)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.invoker"></a>[function <span class="apidocSignatureSpan">ramda.</span>invoker (a, b)](#apidoc.element.ramda.invoker)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.is"></a>[function <span class="apidocSignatureSpan">ramda.</span>is (a, b)](#apidoc.element.ramda.is)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.isArrayLike"></a>[function <span class="apidocSignatureSpan">ramda.</span>isArrayLike (a)](#apidoc.element.ramda.isArrayLike)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.isEmpty"></a>[function <span class="apidocSignatureSpan">ramda.</span>isEmpty (a)](#apidoc.element.ramda.isEmpty)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.isNil"></a>[function <span class="apidocSignatureSpan">ramda.</span>isNil (a)](#apidoc.element.ramda.isNil)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.join"></a>[function <span class="apidocSignatureSpan">ramda.</span>join (a0, a1)](#apidoc.element.ramda.join)
- description and source-code
```javascript
join = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.juxt"></a>[function <span class="apidocSignatureSpan">ramda.</span>juxt (a)](#apidoc.element.ramda.juxt)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.keys"></a>[function <span class="apidocSignatureSpan">ramda.</span>keys (a)](#apidoc.element.ramda.keys)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.keysIn"></a>[function <span class="apidocSignatureSpan">ramda.</span>keysIn (a)](#apidoc.element.ramda.keysIn)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.last"></a>[function <span class="apidocSignatureSpan">ramda.</span>last (a)](#apidoc.element.ramda.last)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.lastIndexOf"></a>[function <span class="apidocSignatureSpan">ramda.</span>lastIndexOf (a, b)](#apidoc.element.ramda.lastIndexOf)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.length"></a>[function <span class="apidocSignatureSpan">ramda.</span>length (a)](#apidoc.element.ramda.length)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.lens"></a>[function <span class="apidocSignatureSpan">ramda.</span>lens (a, b)](#apidoc.element.ramda.lens)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.lensIndex"></a>[function <span class="apidocSignatureSpan">ramda.</span>lensIndex (a)](#apidoc.element.ramda.lensIndex)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.lensPath"></a>[function <span class="apidocSignatureSpan">ramda.</span>lensPath (a)](#apidoc.element.ramda.lensPath)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.lensProp"></a>[function <span class="apidocSignatureSpan">ramda.</span>lensProp (a)](#apidoc.element.ramda.lensProp)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.lift"></a>[function <span class="apidocSignatureSpan">ramda.</span>lift (a)](#apidoc.element.ramda.lift)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.liftN"></a>[function <span class="apidocSignatureSpan">ramda.</span>liftN (a, b)](#apidoc.element.ramda.liftN)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.lt"></a>[function <span class="apidocSignatureSpan">ramda.</span>lt (a, b)](#apidoc.element.ramda.lt)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.lte"></a>[function <span class="apidocSignatureSpan">ramda.</span>lte (a, b)](#apidoc.element.ramda.lte)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.map"></a>[function <span class="apidocSignatureSpan">ramda.</span>map (a, b)](#apidoc.element.ramda.map)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.mapAccum"></a>[function <span class="apidocSignatureSpan">ramda.</span>mapAccum (a, b, c)](#apidoc.element.ramda.mapAccum)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.mapAccumRight"></a>[function <span class="apidocSignatureSpan">ramda.</span>mapAccumRight (a, b, c)](#apidoc.element.ramda.mapAccumRight)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.mapObjIndexed"></a>[function <span class="apidocSignatureSpan">ramda.</span>mapObjIndexed (a, b)](#apidoc.element.ramda.mapObjIndexed)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.match"></a>[function <span class="apidocSignatureSpan">ramda.</span>match (a, b)](#apidoc.element.ramda.match)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.mathMod"></a>[function <span class="apidocSignatureSpan">ramda.</span>mathMod (a, b)](#apidoc.element.ramda.mathMod)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.max"></a>[function <span class="apidocSignatureSpan">ramda.</span>max (a, b)](#apidoc.element.ramda.max)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.maxBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>maxBy (a, b, c)](#apidoc.element.ramda.maxBy)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.mean"></a>[function <span class="apidocSignatureSpan">ramda.</span>mean (a)](#apidoc.element.ramda.mean)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.median"></a>[function <span class="apidocSignatureSpan">ramda.</span>median (a)](#apidoc.element.ramda.median)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.memoize"></a>[function <span class="apidocSignatureSpan">ramda.</span>memoize (a)](#apidoc.element.ramda.memoize)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.merge"></a>[function <span class="apidocSignatureSpan">ramda.</span>merge (a, b)](#apidoc.element.ramda.merge)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.mergeAll"></a>[function <span class="apidocSignatureSpan">ramda.</span>mergeAll (a)](#apidoc.element.ramda.mergeAll)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.mergeWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>mergeWith (a, b, c)](#apidoc.element.ramda.mergeWith)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.mergeWithKey"></a>[function <span class="apidocSignatureSpan">ramda.</span>mergeWithKey (a, b, c)](#apidoc.element.ramda.mergeWithKey)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.min"></a>[function <span class="apidocSignatureSpan">ramda.</span>min (a, b)](#apidoc.element.ramda.min)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.minBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>minBy (a, b, c)](#apidoc.element.ramda.minBy)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.modulo"></a>[function <span class="apidocSignatureSpan">ramda.</span>modulo (a, b)](#apidoc.element.ramda.modulo)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.multiply"></a>[function <span class="apidocSignatureSpan">ramda.</span>multiply (a, b)](#apidoc.element.ramda.multiply)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.nAry"></a>[function <span class="apidocSignatureSpan">ramda.</span>nAry (a, b)](#apidoc.element.ramda.nAry)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.negate"></a>[function <span class="apidocSignatureSpan">ramda.</span>negate (a)](#apidoc.element.ramda.negate)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.none"></a>[function <span class="apidocSignatureSpan">ramda.</span>none (a, b)](#apidoc.element.ramda.none)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.not"></a>[function <span class="apidocSignatureSpan">ramda.</span>not (a)](#apidoc.element.ramda.not)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.nth"></a>[function <span class="apidocSignatureSpan">ramda.</span>nth (a, b)](#apidoc.element.ramda.nth)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.nthArg"></a>[function <span class="apidocSignatureSpan">ramda.</span>nthArg (a)](#apidoc.element.ramda.nthArg)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.objOf"></a>[function <span class="apidocSignatureSpan">ramda.</span>objOf (a, b)](#apidoc.element.ramda.objOf)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.of"></a>[function <span class="apidocSignatureSpan">ramda.</span>of (a)](#apidoc.element.ramda.of)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.omit"></a>[function <span class="apidocSignatureSpan">ramda.</span>omit (a, b)](#apidoc.element.ramda.omit)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.once"></a>[function <span class="apidocSignatureSpan">ramda.</span>once (a)](#apidoc.element.ramda.once)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.or"></a>[function <span class="apidocSignatureSpan">ramda.</span>or (a, b)](#apidoc.element.ramda.or)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.over"></a>[function <span class="apidocSignatureSpan">ramda.</span>over (a, b, c)](#apidoc.element.ramda.over)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pair"></a>[function <span class="apidocSignatureSpan">ramda.</span>pair (a, b)](#apidoc.element.ramda.pair)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.partial"></a>[function <span class="apidocSignatureSpan">ramda.</span>partial (a, b)](#apidoc.element.ramda.partial)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.partialRight"></a>[function <span class="apidocSignatureSpan">ramda.</span>partialRight (a, b)](#apidoc.element.ramda.partialRight)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.partition"></a>[function <span class="apidocSignatureSpan">ramda.</span>partition (a0, a1)](#apidoc.element.ramda.partition)
- description and source-code
```javascript
partition = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.path"></a>[function <span class="apidocSignatureSpan">ramda.</span>path (a, b)](#apidoc.element.ramda.path)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pathEq"></a>[function <span class="apidocSignatureSpan">ramda.</span>pathEq (a, b, c)](#apidoc.element.ramda.pathEq)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pathOr"></a>[function <span class="apidocSignatureSpan">ramda.</span>pathOr (a, b, c)](#apidoc.element.ramda.pathOr)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pathSatisfies"></a>[function <span class="apidocSignatureSpan">ramda.</span>pathSatisfies (a, b, c)](#apidoc.element.ramda.pathSatisfies)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pick"></a>[function <span class="apidocSignatureSpan">ramda.</span>pick (a, b)](#apidoc.element.ramda.pick)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pickAll"></a>[function <span class="apidocSignatureSpan">ramda.</span>pickAll (a, b)](#apidoc.element.ramda.pickAll)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pickBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>pickBy (a, b)](#apidoc.element.ramda.pickBy)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pipe"></a>[function <span class="apidocSignatureSpan">ramda.</span>pipe ()](#apidoc.element.ramda.pipe)
- description and source-code
```javascript
function pipe() {
  if (arguments.length === 0) {
    throw new Error('pipe requires at least one argument');
  }
  return _arity(arguments[0].length,
                reduce(_pipe, arguments[0], tail(arguments)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pipeK"></a>[function <span class="apidocSignatureSpan">ramda.</span>pipeK ()](#apidoc.element.ramda.pipeK)
- description and source-code
```javascript
function pipeK() {
  if (arguments.length === 0) {
    throw new Error('pipeK requires at least one argument');
  }
  return composeK.apply(this, reverse(arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pipeP"></a>[function <span class="apidocSignatureSpan">ramda.</span>pipeP ()](#apidoc.element.ramda.pipeP)
- description and source-code
```javascript
function pipeP() {
  if (arguments.length === 0) {
    throw new Error('pipeP requires at least one argument');
  }
  return _arity(arguments[0].length,
                reduce(_pipeP, arguments[0], tail(arguments)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.pluck"></a>[function <span class="apidocSignatureSpan">ramda.</span>pluck (a, b)](#apidoc.element.ramda.pluck)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.prepend"></a>[function <span class="apidocSignatureSpan">ramda.</span>prepend (a, b)](#apidoc.element.ramda.prepend)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.product"></a>[function <span class="apidocSignatureSpan">ramda.</span>product (a)](#apidoc.element.ramda.product)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.project"></a>[function <span class="apidocSignatureSpan">ramda.</span>project (a0, a1)](#apidoc.element.ramda.project)
- description and source-code
```javascript
project = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.prop"></a>[function <span class="apidocSignatureSpan">ramda.</span>prop (a, b)](#apidoc.element.ramda.prop)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.propEq"></a>[function <span class="apidocSignatureSpan">ramda.</span>propEq (a, b, c)](#apidoc.element.ramda.propEq)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.propIs"></a>[function <span class="apidocSignatureSpan">ramda.</span>propIs (a, b, c)](#apidoc.element.ramda.propIs)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.propOr"></a>[function <span class="apidocSignatureSpan">ramda.</span>propOr (a, b, c)](#apidoc.element.ramda.propOr)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.propSatisfies"></a>[function <span class="apidocSignatureSpan">ramda.</span>propSatisfies (a, b, c)](#apidoc.element.ramda.propSatisfies)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.props"></a>[function <span class="apidocSignatureSpan">ramda.</span>props (a, b)](#apidoc.element.ramda.props)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.range"></a>[function <span class="apidocSignatureSpan">ramda.</span>range (a, b)](#apidoc.element.ramda.range)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.reduce"></a>[function <span class="apidocSignatureSpan">ramda.</span>reduce (a, b, c)](#apidoc.element.ramda.reduce)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.reduceBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>reduceBy ()](#apidoc.element.ramda.reduceBy)
- description and source-code
```javascript
reduceBy = function () {
  var combined = [];
  var argsIdx = 0;
  var left = length;
  var combinedIdx = 0;
  while (combinedIdx < received.length || argsIdx < arguments.length) {
    var result;
    if (combinedIdx < received.length &&
        (!_isPlaceholder(received[combinedIdx]) ||
         argsIdx >= arguments.length)) {
      result = received[combinedIdx];
    } else {
      result = arguments[argsIdx];
      argsIdx += 1;
    }
    combined[combinedIdx] = result;
    if (!_isPlaceholder(result)) {
      left -= 1;
    }
    combinedIdx += 1;
  }
  return left <= 0 ? fn.apply(this, combined)
                   : _arity(left, _curryN(length, combined, fn));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.reduceRight"></a>[function <span class="apidocSignatureSpan">ramda.</span>reduceRight (a, b, c)](#apidoc.element.ramda.reduceRight)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.reduceWhile"></a>[function <span class="apidocSignatureSpan">ramda.</span>reduceWhile ()](#apidoc.element.ramda.reduceWhile)
- description and source-code
```javascript
reduceWhile = function () {
  var combined = [];
  var argsIdx = 0;
  var left = length;
  var combinedIdx = 0;
  while (combinedIdx < received.length || argsIdx < arguments.length) {
    var result;
    if (combinedIdx < received.length &&
        (!_isPlaceholder(received[combinedIdx]) ||
         argsIdx >= arguments.length)) {
      result = received[combinedIdx];
    } else {
      result = arguments[argsIdx];
      argsIdx += 1;
    }
    combined[combinedIdx] = result;
    if (!_isPlaceholder(result)) {
      left -= 1;
    }
    combinedIdx += 1;
  }
  return left <= 0 ? fn.apply(this, combined)
                   : _arity(left, _curryN(length, combined, fn));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.reduced"></a>[function <span class="apidocSignatureSpan">ramda.</span>reduced (a)](#apidoc.element.ramda.reduced)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.reject"></a>[function <span class="apidocSignatureSpan">ramda.</span>reject (a, b)](#apidoc.element.ramda.reject)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.remove"></a>[function <span class="apidocSignatureSpan">ramda.</span>remove (a, b, c)](#apidoc.element.ramda.remove)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.repeat"></a>[function <span class="apidocSignatureSpan">ramda.</span>repeat (a, b)](#apidoc.element.ramda.repeat)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.replace"></a>[function <span class="apidocSignatureSpan">ramda.</span>replace (a, b, c)](#apidoc.element.ramda.replace)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.reverse"></a>[function <span class="apidocSignatureSpan">ramda.</span>reverse (a)](#apidoc.element.ramda.reverse)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.scan"></a>[function <span class="apidocSignatureSpan">ramda.</span>scan (a, b, c)](#apidoc.element.ramda.scan)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.sequence"></a>[function <span class="apidocSignatureSpan">ramda.</span>sequence (a, b)](#apidoc.element.ramda.sequence)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.set"></a>[function <span class="apidocSignatureSpan">ramda.</span>set (a, b, c)](#apidoc.element.ramda.set)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.slice"></a>[function <span class="apidocSignatureSpan">ramda.</span>slice (a, b, c)](#apidoc.element.ramda.slice)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.sort"></a>[function <span class="apidocSignatureSpan">ramda.</span>sort (a, b)](#apidoc.element.ramda.sort)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.sortBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>sortBy (a, b)](#apidoc.element.ramda.sortBy)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.sortWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>sortWith (a, b)](#apidoc.element.ramda.sortWith)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.split"></a>[function <span class="apidocSignatureSpan">ramda.</span>split (a0, a1)](#apidoc.element.ramda.split)
- description and source-code
```javascript
split = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.splitAt"></a>[function <span class="apidocSignatureSpan">ramda.</span>splitAt (a, b)](#apidoc.element.ramda.splitAt)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.splitEvery"></a>[function <span class="apidocSignatureSpan">ramda.</span>splitEvery (a, b)](#apidoc.element.ramda.splitEvery)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.splitWhen"></a>[function <span class="apidocSignatureSpan">ramda.</span>splitWhen (a, b)](#apidoc.element.ramda.splitWhen)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.subtract"></a>[function <span class="apidocSignatureSpan">ramda.</span>subtract (a, b)](#apidoc.element.ramda.subtract)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.sum"></a>[function <span class="apidocSignatureSpan">ramda.</span>sum (a)](#apidoc.element.ramda.sum)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.symmetricDifference"></a>[function <span class="apidocSignatureSpan">ramda.</span>symmetricDifference (a, b)](#apidoc.element.ramda.symmetricDifference)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.symmetricDifferenceWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>symmetricDifferenceWith (a, b, c)](#apidoc.element.ramda.symmetricDifferenceWith)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.tail"></a>[function <span class="apidocSignatureSpan">ramda.</span>tail (a)](#apidoc.element.ramda.tail)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.take"></a>[function <span class="apidocSignatureSpan">ramda.</span>take (a, b)](#apidoc.element.ramda.take)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.takeLast"></a>[function <span class="apidocSignatureSpan">ramda.</span>takeLast (a, b)](#apidoc.element.ramda.takeLast)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.takeLastWhile"></a>[function <span class="apidocSignatureSpan">ramda.</span>takeLastWhile (a, b)](#apidoc.element.ramda.takeLastWhile)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.takeWhile"></a>[function <span class="apidocSignatureSpan">ramda.</span>takeWhile (a, b)](#apidoc.element.ramda.takeWhile)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.tap"></a>[function <span class="apidocSignatureSpan">ramda.</span>tap (a, b)](#apidoc.element.ramda.tap)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.test"></a>[function <span class="apidocSignatureSpan">ramda.</span>test (a, b)](#apidoc.element.ramda.test)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.times"></a>[function <span class="apidocSignatureSpan">ramda.</span>times (a, b)](#apidoc.element.ramda.times)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.toLower"></a>[function <span class="apidocSignatureSpan">ramda.</span>toLower (a)](#apidoc.element.ramda.toLower)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.toPairs"></a>[function <span class="apidocSignatureSpan">ramda.</span>toPairs (a)](#apidoc.element.ramda.toPairs)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.toPairsIn"></a>[function <span class="apidocSignatureSpan">ramda.</span>toPairsIn (a)](#apidoc.element.ramda.toPairsIn)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.toUpper"></a>[function <span class="apidocSignatureSpan">ramda.</span>toUpper (a)](#apidoc.element.ramda.toUpper)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.transduce"></a>[function <span class="apidocSignatureSpan">ramda.</span>transduce (a0, a1, a2, a3)](#apidoc.element.ramda.transduce)
- description and source-code
```javascript
transduce = function (a0, a1, a2, a3) { return fn.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.transpose"></a>[function <span class="apidocSignatureSpan">ramda.</span>transpose (a)](#apidoc.element.ramda.transpose)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.traverse"></a>[function <span class="apidocSignatureSpan">ramda.</span>traverse (a, b, c)](#apidoc.element.ramda.traverse)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.trim"></a>[function <span class="apidocSignatureSpan">ramda.</span>trim (a)](#apidoc.element.ramda.trim)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.tryCatch"></a>[function <span class="apidocSignatureSpan">ramda.</span>tryCatch (a, b)](#apidoc.element.ramda.tryCatch)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.type"></a>[function <span class="apidocSignatureSpan">ramda.</span>type (a)](#apidoc.element.ramda.type)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.unapply"></a>[function <span class="apidocSignatureSpan">ramda.</span>unapply (a)](#apidoc.element.ramda.unapply)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.unary"></a>[function <span class="apidocSignatureSpan">ramda.</span>unary (a)](#apidoc.element.ramda.unary)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.uncurryN"></a>[function <span class="apidocSignatureSpan">ramda.</span>uncurryN (a, b)](#apidoc.element.ramda.uncurryN)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.unfold"></a>[function <span class="apidocSignatureSpan">ramda.</span>unfold (a, b)](#apidoc.element.ramda.unfold)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.union"></a>[function <span class="apidocSignatureSpan">ramda.</span>union (a, b)](#apidoc.element.ramda.union)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.unionWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>unionWith (a, b, c)](#apidoc.element.ramda.unionWith)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.uniq"></a>[function <span class="apidocSignatureSpan">ramda.</span>uniq (a)](#apidoc.element.ramda.uniq)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.uniqBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>uniqBy (a, b)](#apidoc.element.ramda.uniqBy)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.uniqWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>uniqWith (a, b)](#apidoc.element.ramda.uniqWith)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.unless"></a>[function <span class="apidocSignatureSpan">ramda.</span>unless (a, b, c)](#apidoc.element.ramda.unless)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.unnest"></a>[function <span class="apidocSignatureSpan">ramda.</span>unnest (a)](#apidoc.element.ramda.unnest)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.until"></a>[function <span class="apidocSignatureSpan">ramda.</span>until (a, b, c)](#apidoc.element.ramda.until)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.update"></a>[function <span class="apidocSignatureSpan">ramda.</span>update (a, b, c)](#apidoc.element.ramda.update)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.useWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>useWith (a, b)](#apidoc.element.ramda.useWith)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.values"></a>[function <span class="apidocSignatureSpan">ramda.</span>values (a)](#apidoc.element.ramda.values)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.valuesIn"></a>[function <span class="apidocSignatureSpan">ramda.</span>valuesIn (a)](#apidoc.element.ramda.valuesIn)
- description and source-code
```javascript
function f1(a) {
  if (arguments.length === 0 || _isPlaceholder(a)) {
    return f1;
  } else {
    return fn.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.view"></a>[function <span class="apidocSignatureSpan">ramda.</span>view (a, b)](#apidoc.element.ramda.view)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.when"></a>[function <span class="apidocSignatureSpan">ramda.</span>when (a, b, c)](#apidoc.element.ramda.when)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.where"></a>[function <span class="apidocSignatureSpan">ramda.</span>where (a, b)](#apidoc.element.ramda.where)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.whereEq"></a>[function <span class="apidocSignatureSpan">ramda.</span>whereEq (a, b)](#apidoc.element.ramda.whereEq)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.without"></a>[function <span class="apidocSignatureSpan">ramda.</span>without (a, b)](#apidoc.element.ramda.without)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.xprod"></a>[function <span class="apidocSignatureSpan">ramda.</span>xprod (a, b)](#apidoc.element.ramda.xprod)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.zip"></a>[function <span class="apidocSignatureSpan">ramda.</span>zip (a, b)](#apidoc.element.ramda.zip)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.zipObj"></a>[function <span class="apidocSignatureSpan">ramda.</span>zipObj (a, b)](#apidoc.element.ramda.zipObj)
- description and source-code
```javascript
function f2(a, b) {
  switch (arguments.length) {
    case 0:
      return f2;
    case 1:
      return _isPlaceholder(a) ? f2
           : _curry1(function(_b) { return fn(a, _b); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f2
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b); })
           : fn(a, b);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ramda.zipWith"></a>[function <span class="apidocSignatureSpan">ramda.</span>zipWith (a, b, c)](#apidoc.element.ramda.zipWith)
- description and source-code
```javascript
function f3(a, b, c) {
  switch (arguments.length) {
    case 0:
      return f3;
    case 1:
      return _isPlaceholder(a) ? f3
           : _curry2(function(_b, _c) { return fn(a, _b, _c); });
    case 2:
      return _isPlaceholder(a) && _isPlaceholder(b) ? f3
           : _isPlaceholder(a) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _curry1(function(_c) { return fn(a, b, _c); });
    default:
      return _isPlaceholder(a) && _isPlaceholder(b) && _isPlaceholder(c) ? f3
           : _isPlaceholder(a) && _isPlaceholder(b) ? _curry2(function(_a, _b) { return fn(_a, _b, c); })
           : _isPlaceholder(a) && _isPlaceholder(c) ? _curry2(function(_a, _c) { return fn(_a, b, _c); })
           : _isPlaceholder(b) && _isPlaceholder(c) ? _curry2(function(_b, _c) { return fn(a, _b, _c); })
           : _isPlaceholder(a) ? _curry1(function(_a) { return fn(_a, b, c); })
           : _isPlaceholder(b) ? _curry1(function(_b) { return fn(a, _b, c); })
           : _isPlaceholder(c) ? _curry1(function(_c) { return fn(a, b, _c); })
           : fn(a, b, c);
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
