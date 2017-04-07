# api documentation for  [ramda (v0.23.0)](http://ramdajs.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-ramda.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ramda) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ramda.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ramda)
#### A practical functional library for JavaScript programmers.

[![NPM](https://nodei.co/npm/ramda.png?downloads=true)](https://www.npmjs.com/package/ramda)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ramda/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-ramda%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ramda/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-ramda/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-ramda/build/screenCapture.npmPackageDependencyTree.svg)



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
...
 * @category Function
 * @sig * -> Boolean
 * @param {*}
 * @return {Boolean}
 * @see R.always, R.T
 * @example
 *
 *      R.F(); //=> false
 */
module.exports = always(false);
...
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
...
 * @category Function
 * @sig * -> Boolean
 * @param {*}
 * @return {Boolean}
 * @see R.always, R.F
 * @example
 *
 *      R.T(); //=> true
 */
module.exports = always(true);
...
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
...
 * @sig Number -> Number -> Number
 * @param {Number} a
 * @param {Number} b
 * @return {Number}
 * @see R.subtract
 * @example
 *
 *      R.add(2, 3);       //=>  5
 *      R.add(7)(10);      //=> 17
 */
module.exports = _curry2(function add(a, b) {
  return Number(a) + Number(b);
});
...
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
...
 * @category Function
 * @category List
 * @sig ((a ... -> b) ... -> [a] -> *) -> (a ..., Int, [a] -> b) ... -> [a] -> *)
 * @param {Function} fn A list iteration function that does not pass index or list to its callback
 * @return {Function} An altered list iteration function that passes (item, index, list) to its callback
 * @example
 *
 *      var mapIndexed = R.addIndex(R.map);
 *      mapIndexed((val, idx) => idx + '-' + val, ['f', 'o', 'o', 'b', 'a', 'r']);
 *      //=> ['0-f', '1-o', '2-o', '3-b', '4-a', '5-r']
 */
module.exports = _curry1(function addIndex(fn) {
return curryN(fn.length, function() {
  var idx = 0;
  var origFn = arguments[0];
...
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
...
 *        at the supplied index will be replaced.
 * @return {Array} A copy of the supplied array-like object with
 *         the element at index 'idx' replaced with the value
 *         returned by applying 'fn' to the existing element.
 * @see R.update
 * @example
 *
 *      R.adjust(R.add(10), 1, [1, 2, 3]);     //=> [1, 12, 3]
 *      R.adjust(R.add(10))(1)([1, 2, 3]);     //=> [1, 12, 3]
 * @symb R.adjust(f, -1, [a, b]) = [a, f(b)]
 * @symb R.adjust(f, 0, [a, b]) = [f(a), b]
 */
module.exports = _curry3(function adjust(fn, idx, list) {
if (idx >= list.length || idx < -list.length) {
  return list;
...
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
...
 * @param {Array} list The array to consider.
 * @return {Boolean} 'true' if the predicate is satisfied by every element, 'false'
 *         otherwise.
 * @see R.any, R.none, R.transduce
 * @example
 *
 *      var equals3 = R.equals(3);
 *      R.all(equals3)([3, 3, 3, 3]); //=> true
 *      R.all(equals3)([3, 3, 1, 3]); //=> false
 */
module.exports = _curry2(_dispatchable(['all'], _xall, function all(fn, list) {
var idx = 0;
while (idx < list.length) {
  if (!fn(list[idx])) {
    return false;
...
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
...
 * @param {Array} predicates An array of predicates to check
 * @return {Function} The combined predicate
 * @see R.anyPass
 * @example
 *
 *      var isQueen = R.propEq('rank', 'Q');
 *      var isSpade = R.propEq('suit', '♠︎');
 *      var isQueenOfSpades = R.allPass([isQueen, isSpade]);
 *
 *      isQueenOfSpades({rank: 'Q', suit: '♣︎'}); //=> false
 *      isQueenOfSpades({rank: 'Q', suit: '♠︎'}); //=> true
 */
module.exports = _curry1(function allPass(preds) {
return curryN(reduce(max, 0, pluck('length', preds)), function() {
  var idx = 0;
...
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
...
 * @since v0.1.0
 * @category Function
 * @sig a -> (* -> a)
 * @param {*} val The value to wrap in a function
 * @return {Function} A Function :: * -> val.
 * @example
 *
 *      var t = R.always('Tee');
 *      t(); //=> 'Tee'
 */
module.exports = _curry1(function always(val) {
  return function() {
    return val;
  };
});
...
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
...
 * @sig a -> b -> a | b
 * @param {Any} a
 * @param {Any} b
 * @return {Any} the first argument if it is falsy, otherwise the second argument.
 * @see R.both
 * @example
 *
 *      R.and(true, true); //=> true
 *      R.and(true, false); //=> false
 *      R.and(false, true); //=> false
 *      R.and(false, false); //=> false
 */
module.exports = _curry2(function and(a, b) {
  return a && b;
});
...
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
...
 * @return {Boolean} 'true' if the predicate is satisfied by at least one element, 'false'
 *         otherwise.
 * @see R.all, R.none, R.transduce
 * @example
 *
 *      var lessThan0 = R.flip(R.lt)(0);
 *      var lessThan2 = R.flip(R.lt)(2);
 *      R.any(lessThan0)([1, 2]); //=> false
 *      R.any(lessThan2)([1, 2]); //=> true
 */
module.exports = _curry2(_dispatchable(['any'], _xany, function any(fn, list) {
var idx = 0;
while (idx < list.length) {
  if (fn(list[idx])) {
    return true;
...
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
...
 * @param {Array} predicates An array of predicates to check
 * @return {Function} The combined predicate
 * @see R.allPass
 * @example
 *
 *      var isClub = R.propEq('suit', '♣');
 *      var isSpade = R.propEq('suit', '♠');
 *      var isBlackCard = R.anyPass([isClub, isSpade]);
 *
 *      isBlackCard({rank: '10', suit: '♣'}); //=> true
 *      isBlackCard({rank: 'Q', suit: '♠'}); //=> true
 *      isBlackCard({rank: 'Q', suit: '♦'}); //=> false
 */
module.exports = _curry1(function anyPass(preds) {
return curryN(reduce(max, 0, pluck('length', preds)), function() {
...
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
...
 * @sig [a -> b] -> [a] -> [b]
 * @sig Apply f => f (a -> b) -> f a -> f b
 * @param {Array} fns An array of functions
 * @param {Array} vs An array of values
 * @return {Array} An array of results of applying each of 'fns' to all of 'vs' in turn.
 * @example
 *
 *      R.ap([R.multiply(2), R.add(3)], [1,2,3]); //=> [2, 4, 6, 4, 5, 6]
 *      R.ap([R.concat('tasty '), R.toUpper], ['pizza', 'salad']); //=> ["tasty pizza", "tasty salad", "PIZZA", "SALAD"]
 * @symb R.ap([f, g], [a, b]) = [f(a), f(b), g(a), g(b)]
 */
module.exports = _curry2(function ap(applicative, fn) {
return (
  typeof applicative.ap === 'function' ?
    applicative.ap(fn) :
...
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
...
 * @sig Number -> [a] -> [[a]]
 * @param {Number} n The size of the tuples to create
 * @param {Array} list The list to split into 'n'-length tuples
 * @return {Array} The resulting list of 'n'-length tuples
 * @see R.transduce
 * @example
 *
 *      R.aperture(2, [1, 2, 3, 4, 5]); //=> [[1, 2], [2, 3], [3, 4], [4, 5]]
 *      R.aperture(3, [1, 2, 3, 4, 5]); //=> [[1, 2, 3], [2, 3, 4], [3, 4, 5]]
 *      R.aperture(7, [1, 2, 3, 4, 5]); //=> []
 */
module.exports = _curry2(_dispatchable([], _xaperture, _aperture));
...
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
...
 * @param {*} el The element to add to the end of the new list.
 * @param {Array} list The list of elements to add a new item to.
 *        list.
 * @return {Array} A new list containing the elements of the old list followed by 'el'.
 * @see R.prepend
 * @example
 *
 *      R.append('tests', ['write', 'more']); //=> ['write', 'more', 'tests']
 *      R.append('tests', []); //=> ['tests']
 *      R.append(['tests'], ['write', 'more']); //=> ['write', 'more', ['tests']]
 */
module.exports = _curry2(function append(el, list) {
  return _concat(list, [el]);
});
...
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
...
module.exports = _curry1(function addIndex(fn) {
  return curryN(fn.length, function() {
    var idx = 0;
    var origFn = arguments[0];
    var list = arguments[arguments.length - 1];
    var args = Array.prototype.slice.call(arguments, 0);
    args[0] = function() {
      var result = origFn.apply(this, _concat(arguments, [idx, list]));
      idx += 1;
      return result;
    };
    return fn.apply(this, args);
  });
});
...
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
...
 *        producing the values for these properties.
 * @return {Function} A function that returns an object of the same structure
 * as 'spec', with each property set to the value returned by calling its
 * associated function with the supplied arguments.
 * @see R.converge, R.juxt
 * @example
 *
 *      var getMetrics = R.applySpec({
 *                                      sum: R.add,
 *                                      nested: { mul: R.multiply }
 *                                   });
 *      getMetrics(2, 4); // => { sum: 6, nested: { mul: 8 } }
 * @symb R.applySpec({ x: f, y: { z: g } })(a, b) = { x: f(a, b), y: { z: g(a, b) } }
 */
module.exports = _curry1(function applySpec(spec) {
...
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
...
 * @sig Ord b => (a -> b) -> a -> a -> Number
 * @param {Function} fn A function of arity one that returns a value that can be compared
 * @param {*} a The first item to be compared.
 * @param {*} b The second item to be compared.
 * @return {Number} '-1' if fn(a) < fn(b), '1' if fn(b) < fn(a), otherwise '0'
 * @example
 *
 *      var byAge = R.ascend(R.prop('age'));
 *      var people = [
 *        // ...
 *      ];
 *      var peopleByYoungestFirst = R.sort(byAge, people);
 */
module.exports = _curry3(function ascend(fn, a, b) {
var aa = fn(a);
...
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
...
 * @param {String} prop The property name to set
 * @param {*} val The new value
 * @param {Object} obj The object to clone
 * @return {Object} A new object equivalent to the original except for the changed property.
 * @see R.dissoc
 * @example
 *
 *      R.assoc('c', 3, {a: 1, b: 2}); //=> {a: 1, b: 2, c: 3}
 */
module.exports = _curry3(function assoc(prop, val, obj) {
var result = {};
for (var p in obj) {
  result[p] = obj[p];
}
result[prop] = val;
...
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
...
 * @param {Array} path the path to set
 * @param {*} val The new value
 * @param {Object} obj The object to clone
 * @return {Object} A new object equivalent to the original except along the specified path.
 * @see R.dissocPath
 * @example
 *
 *      R.assocPath(['a', 'b', 'c'], 42, {a: {b: {c: 0}}}); //=> {a: {b: {c: 42}}}
 *
 *      // Any missing or non-object keys in path will be overridden
 *      R.assocPath(['a', 'b', 'c'], 42, {a: 5}); //=> {a: {b: {c: 42}}}
 */
module.exports = _curry3(function assocPath(path, val, obj) {
if (path.length === 0) {
  return val;
...
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
...
 *
 *      var takesThreeArgs = function(a, b, c) {
 *        return [a, b, c];
 *      };
 *      takesThreeArgs.length; //=> 3
 *      takesThreeArgs(1, 2, 3); //=> [1, 2, 3]
 *
 *      var takesTwoArgs = R.binary(takesThreeArgs);
 *      takesTwoArgs.length; //=> 2
 *      // Only 2 arguments are passed to the wrapped function
 *      takesTwoArgs(1, 2, 3); //=> [1, 2, undefined]
 * @symb R.binary(f)(a, b, c) = f(a, b)
 */
module.exports = _curry1(function binary(fn) {
return nAry(2, fn);
...
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
...
 * @sig (* -> *) -> {*} -> (* -> *)
 * @param {Function} fn The function to bind to context
 * @param {Object} thisObj The context to bind 'fn' to
 * @return {Function} A function that will execute in the context of 'thisObj'.
 * @see R.partial
 * @example
 *
 *      var log = R.bind(console.log, console);
 *      R.pipe(R.assoc('a', 2), R.tap(log), R.assoc('a', 3))({a: 1}); //=> {a: 3}
 *      // logs {a: 2}
 * @symb R.bind(f, o)(a, b) = f.call(o, a, b)
 */
module.exports = _curry2(function bind(fn, thisObj) {
return _arity(fn.length, function() {
  return fn.apply(thisObj, arguments);
...
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
...
 * @param {Function} g Another predicate
 * @return {Function} a function that applies its arguments to 'f' and 'g' and '&&'s their outputs together.
 * @see R.and
 * @example
 *
 *      var gt10 = R.gt(R.__, 10)
 *      var lt20 = R.lt(R.__, 20)
 *      var f = R.both(gt10, lt20);
 *      f(15); //=> true
 *      f(30); //=> false
 */
module.exports = _curry2(function both(f, g) {
return _isFunction(f) ?
  function _both() {
    return f.apply(this, arguments) && g.apply(this, arguments);
...
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
...
 *      //=> ['0-f', '1-o', '2-o', '3-b', '4-a', '5-r']
 */
module.exports = _curry1(function addIndex(fn) {
return curryN(fn.length, function() {
  var idx = 0;
  var origFn = arguments[0];
  var list = arguments[arguments.length - 1];
  var args = Array.prototype.slice.call(arguments, 0);
  args[0] = function() {
    var result = origFn.apply(this, _concat(arguments, [idx, list]));
    idx += 1;
    return result;
  };
  return fn.apply(this, args);
});
...
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
...
 * @sig Chain m => (a -> m b) -> m a -> m b
 * @param {Function} fn The function to map with
 * @param {Array} list The list to map over
 * @return {Array} The result of flat-mapping 'list' with 'fn'
 * @example
 *
 *      var duplicate = n => [n, n];
 *      R.chain(duplicate, [1, 2, 3]); //=> [1, 1, 2, 2, 3, 3]
 *
 *      R.chain(R.append, R.head)([1, 2, 3]); //=> [1, 2, 3, 1]
 */
module.exports = _curry2(_dispatchable(['chain'], _xchain, function chain(fn, monad) {
if (typeof monad === 'function') {
  return function(x) { return fn(monad(x))(x); };
}
...
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
...
 * @sig Ord a => a -> a -> a -> a
 * @param {Number} minimum The lower limit of the clamp (inclusive)
 * @param {Number} maximum The upper limit of the clamp (inclusive)
 * @param {Number} value Value to be clamped
 * @return {Number} Returns 'minimum' when 'val < minimum', 'maximum' when 'val > maximum', returns 'val' otherwise
 * @example
 *
 *      R.clamp(1, 10, -5) // => 1
 *      R.clamp(1, 10, 15) // => 10
 *      R.clamp(1, 10, 4)  // => 4
 */
module.exports = _curry3(function clamp(min, max, value) {
if (min > max) {
  throw new Error('min must not be greater than max in clamp(min, max, value)');
}
...
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
...
 * @category Object
 * @sig {*} -> {*}
 * @param {*} value The object or array to clone
 * @return {*} A deeply cloned copy of 'val'
 * @example
 *
 *      var objects = [{}, {}, {}];
 *      var objectsClone = R.clone(objects);
 *      objects === objectsClone; //=> false
 *      objects[0] === objectsClone[0]; //=> false
 */
module.exports = _curry1(function clone(value) {
return value != null && typeof value.clone === 'function' ?
  value.clone() :
  _clone(value, [], [], true);
...
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
...
 * @category Function
 * @sig (a, b -> Boolean) -> (a, b -> Number)
 * @param {Function} pred A predicate function of arity two which will return 'true' if the first argument
 * is less than the second, 'false' otherwise
 * @return {Function} A Function :: a -> b -> Int that returns '-1' if a < b, '1' if b < a, otherwise '0'
 * @example
 *
 *      var byAge = R.comparator((a, b) => a.age < b.age);
 *      var people = [
 *        // ...
 *      ];
 *      var peopleByIncreasingAge = R.sort(byAge, people);
 */
module.exports = _curry1(function comparator(pred) {
return function(a, b) {
...
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
...
 * @category Logic
 * @sig (*... -> *) -> (*... -> Boolean)
 * @param {Function} f
 * @return {Function}
 * @see R.not
 * @example
 *
 *      var isNotNil = R.complement(R.isNil);
 *      isNil(null); //=> true
 *      isNotNil(null); //=> false
 *      isNil(7); //=> false
 *      isNotNil(7); //=> true
 */
module.exports = lift(not);
...
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
...
 * @sig ((y -> z), (x -> y), ..., (o -> p), ((a, b, ..., n) -> o)) -> ((a, b, ..., n) -> z)
 * @param {...Function} ...functions The functions to compose
 * @return {Function}
 * @see R.pipe
 * @example
 *
 *      var classyGreeting = (firstName, lastName) => "The name's " + lastName + ", " + firstName + " " + lastName
 *      var yellGreeting = R.compose(R.toUpper, classyGreeting);
 *      yellGreeting('James', 'Bond'); //=> "THE NAME'S BOND, JAMES BOND"
 *
 *      R.compose(Math.abs, R.add(1), R.multiply(2))(-4) //=> 7
 *
 * @symb R.compose(f, g, h)(a, b) = f(g(h(a, b)))
 */
module.exports = function compose() {
...
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
...
var map = require('./map');


/**
* Returns the right-to-left Kleisli composition of the provided functions,
* each of which must return a value of a type supported by ['chain'](#chain).
*
* 'R.composeK(h, g, f)' is equivalent to 'R.compose(R.chain(h), R.chain(g), R.chain(f))'.
*
* @func
* @memberOf R
* @since v0.16.0
* @category Function
* @sig Chain m => ((y -> m z), (x -> m y), ..., (a -> m b)) -> (a -> m z)
* @param {...Function} ...functions The functions to compose
...
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
...
 *
 *      // We'll pretend to do a db lookup which returns a promise
 *      var lookupUser = (userId) => Promise.resolve(db.users[userId])
 *      var lookupFollowers = (user) => Promise.resolve(user.followers)
 *      lookupUser('JOE').then(lookupFollowers)
 *
 *      //  followersForUser :: String -> Promise [UserId]
 *      var followersForUser = R.composeP(lookupFollowers, lookupUser);
 *      followersForUser('JOE').then(followers => console.log('Followers:', followers))
 *      // Followers: ["STEVE","SUZY"]
 */
module.exports = function composeP() {
if (arguments.length === 0) {
  throw new Error('composeP requires at least one argument');
}
...
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
...
 * @sig Apply f => f (a -> b) -> f a -> f b
 * @param {Array} fns An array of functions
 * @param {Array} vs An array of values
 * @return {Array} An array of results of applying each of 'fns' to all of 'vs' in turn.
 * @example
 *
 *      R.ap([R.multiply(2), R.add(3)], [1,2,3]); //=> [2, 4, 6, 4, 5, 6]
 *      R.ap([R.concat('tasty '), R.toUpper], ['pizza', 'salad']); //=> ["tasty pizza", "tasty salad", "PIZZA", "SALAD"]
 * @symb R.ap([f, g], [a, b]) = [f(a), f(b), g(a), g(b)]
 */
module.exports = _curry2(function ap(applicative, fn) {
return (
  typeof applicative.ap === 'function' ?
    applicative.ap(fn) :
  typeof applicative === 'function' ?
...
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
...
* @since v0.6.0
* @category Logic
* @sig [[(*... -> Boolean),(*... -> *)]] -> (*... -> *)
* @param {Array} pairs A list of [predicate, transformer]
* @return {Function}
* @example
*
*      var fn = R.cond([
*        [R.equals(0),   R.always('water freezes at 0°C')],
*        [R.equals(100), R.always('water boils at 100°C')],
*        [R.T,           temp => 'nothing special happens at ' + temp + '°C']
*      ]);
*      fn(0); //=> 'water freezes at 0°C'
*      fn(50); //=> 'nothing special happens at 50°C'
*      fn(100); //=> 'water boils at 100°C'
...
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
...
*      function Animal(kind) {
*        this.kind = kind;
*      };
*      Animal.prototype.sighting = function() {
*        return "It's a " + this.kind + "!";
*      }
*
*      var AnimalConstructor = R.construct(Animal)
*
*      // Notice we no longer need the 'new' keyword:
*      AnimalConstructor('Pig'); //=> {"kind": "Pig", "sighting": function (){...}};
*
*      var animalTypes = ["Lion", "Tiger", "Bear"];
*      var animalSighting = R.invoker(0, 'sighting');
*      var sightNewAnimal = R.compose(animalSighting, AnimalConstructor);
...
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
...
*      Salad.prototype.recipe = function() {
*        var instructions = R.map((ingredient) => (
*          'Add a whollop of ' + ingredient, this.ingredients)
*        )
*        return R.join('\n', instructions)
*      }
*
*      var ThreeLayerSalad = R.constructN(3, Salad)
*
*      // Notice we no longer need the 'new' keyword, and the constructor is curried for 3 arguments.
*      var salad = ThreeLayerSalad('Mayonnaise')('Potato Chips')('Ketchup')
*      console.log(salad.recipe());
*      // Add a whollop of Mayonnaise
*      // Add a whollop of Potato Chips
*      // Add a whollop of Potato Ketchup
...
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
...
 * @sig a -> [a] -> Boolean
 * @param {Object} a The item to compare against.
 * @param {Array} list The array to consider.
 * @return {Boolean} 'true' if an equivalent item is in the list, 'false' otherwise.
 * @see R.any
 * @example
 *
 *      R.contains(3, [1, 2, 3]); //=> true
 *      R.contains(4, [1, 2, 3]); //=> false
 *      R.contains({ name: 'Fred' }, [{ name: 'Fred' }]); //=> true
 *      R.contains([42], [[42]]); //=> true
 */
module.exports = _curry2(_contains);
...
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
...
*
*      R.call(R.add, 1, 2); //=> 3
*
*      var indentN = R.pipe(R.times(R.always(' ')),
*                           R.join(''),
*                           R.replace(/^(?!$)/gm));
*
*      var format = R.converge(R.call, [
*                                  R.pipe(R.prop('indent'), indentN),
*                                  R.prop('value')
*                              ]);
*
*      format({indent: 2, value: 'foo\nbar\nbaz\n'}); //=> '  foo\n  bar\n  baz\n'
* @symb R.call(f, a, b) = f(a, b)
*/
...
```

#### <a name="apidoc.element.ramda.countBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>countBy (a0, a1)](#apidoc.element.ramda.countBy)
- description and source-code
```javascript
countBy = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
...
 * @sig (a -> String) -> [a] -> {*}
 * @param {Function} fn The function used to map values to keys.
 * @param {Array} list The list to count elements from.
 * @return {Object} An object mapping keys to number of occurrences in the list.
 * @example
 *
 *      var numbers = [1.0, 1.1, 1.2, 2.0, 3.0, 2.2];
 *      R.countBy(Math.floor)(numbers);    //=> {'1': 3, '2': 2, '3': 1}
 *
 *      var letters = ['a', 'b', 'A', 'a', 'B', 'c'];
 *      R.countBy(R.toLower)(letters);   //=> {'a': 3, 'b': 2, 'c': 1}
 */
module.exports = reduceBy(function(acc, elem) { return acc + 1; }, 0);
...
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
...
* @sig Chain m => ((y -> m z), (x -> m y), ..., (a -> m b)) -> (a -> m z)
* @param {...Function} ...functions The functions to compose
* @return {Function}
* @see R.pipeK
* @example
*
*       //  get :: String -> Object -> Maybe *
*       var get = R.curry((propName, obj) => Maybe(obj[propName]))
*
*       //  getStateCode :: Maybe String -> Maybe String
*       var getStateCode = R.composeK(
*         R.compose(Maybe.of, R.toUpper),
*         get('state'),
*         get('address'),
*         get('user'),
...
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
...
var _curry2 = require('./internal/_curry2');
var _curryN = require('./internal/_curryN');


/**
* Returns a curried equivalent of the provided function, with the specified
* arity. The curried function has two unusual capabilities. First, its
* arguments needn't be provided one at a time. If 'g' is 'R.curryN(3, f)', the
* following are equivalent:
*
*   - 'g(1)(2)(3)'
*   - 'g(1)(2, 3)'
*   - 'g(1, 2)(3)'
*   - 'g(1, 2, 3)'
*
...
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
...
 * @category Math
 * @sig Number -> Number
 * @param {Number} n
 * @return {Number} n - 1
 * @see R.inc
 * @example
 *
 *      R.dec(42); //=> 41
 */
module.exports = add(-1);
...
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
...
* @category Logic
* @sig a -> b -> a | b
* @param {a} default The default value.
* @param {b} val 'val' will be returned instead of 'default' unless 'val' is 'null', 'undefined' or 'NaN'.
* @return {*} The second value if it is not 'null', 'undefined' or 'NaN', otherwise the default value
* @example
*
*      var defaultTo42 = R.defaultTo(42);
*
*      defaultTo42(null);  //=> 42
*      defaultTo42(undefined);  //=> 42
*      defaultTo42('Ramda');  //=> 'Ramda'
*      // parseInt('string') results in NaN
*      defaultTo42(parseInt('string')); //=> 42
*/
...
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
...
 * @sig Ord b => (a -> b) -> a -> a -> Number
 * @param {Function} fn A function of arity one that returns a value that can be compared
 * @param {*} a The first item to be compared.
 * @param {*} b The second item to be compared.
 * @return {Number} '-1' if fn(a) > fn(b), '1' if fn(b) > fn(a), otherwise '0'
 * @example
 *
 *      var byAge = R.descend(R.prop('age'));
 *      var people = [
 *        // ...
 *      ];
 *      var peopleByOldestFirst = R.sort(byAge, people);
 */
module.exports = _curry3(function descend(fn, a, b) {
var aa = fn(a);
...
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
...
 * @sig [*] -> [*] -> [*]
 * @param {Array} list1 The first list.
 * @param {Array} list2 The second list.
 * @return {Array} The elements in 'list1' that are not in 'list2'.
 * @see R.differenceWith, R.symmetricDifference, R.symmetricDifferenceWith
 * @example
 *
 *      R.difference([1,2,3,4], [7,6,5,4,3]); //=> [1,2]
 *      R.difference([7,6,5,4,3], [1,2,3,4]); //=> [7,6,5]
 *      R.difference([{a: 1}, {b: 2}], [{a: 1}, {c: 3}]) //=> [{b: 2}]
 */
module.exports = _curry2(function difference(first, second) {
var out = [];
var idx = 0;
var firstLen = first.length;
...
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
...
 * @return {Array} The elements in 'list1' that are not in 'list2'.
 * @see R.difference, R.symmetricDifference, R.symmetricDifferenceWith
 * @example
 *
 *      var cmp = (x, y) => x.a === y.a;
 *      var l1 = [{a: 1}, {a: 2}, {a: 3}];
 *      var l2 = [{a: 3}, {a: 4}];
 *      R.differenceWith(cmp, l1, l2); //=> [{a: 1}, {a: 2}]
 */
module.exports = _curry3(function differenceWith(pred, first, second) {
var out = [];
var idx = 0;
var firstLen = first.length;
while (idx < firstLen) {
  if (!_containsWith(pred, first[idx], second) &&
...
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
...
 * @sig String -> {k: v} -> {k: v}
 * @param {String} prop The name of the property to dissociate
 * @param {Object} obj The object to clone
 * @return {Object} A new object equivalent to the original but without the specified property
 * @see R.assoc
 * @example
 *
 *      R.dissoc('b', {a: 1, b: 2, c: 3}); //=> {a: 1, c: 3}
 */
module.exports = _curry2(function dissoc(prop, obj) {
var result = {};
for (var p in obj) {
  result[p] = obj[p];
}
delete result[prop];
...
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
...
 * @sig [String] -> {k: v} -> {k: v}
 * @param {Array} path The path to the value to omit
 * @param {Object} obj The object to clone
 * @return {Object} A new object without the property at path
 * @see R.assocPath
 * @example
 *
 *      R.dissocPath(['a', 'b', 'c'], {a: {b: {c: 42}}}); //=> {a: {b: {}}}
 */
module.exports = _curry2(function dissocPath(path, obj) {
switch (path.length) {
  case 0:
    return obj;
  case 1:
    return dissoc(path[0], obj);
...
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
...
* @sig Number -> Number -> Number
* @param {Number} a The first value.
* @param {Number} b The second value.
* @return {Number} The result of 'a / b'.
* @see R.multiply
* @example
*
*      R.divide(71, 100); //=> 0.71
*
*      var half = R.divide(R.__, 2);
*      half(42); //=> 21
*
*      var reciprocal = R.divide(1);
*      reciprocal(4);   //=> 0.25
*/
...
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
...
 * @sig Number -> String -> String
 * @param {Number} n
 * @param {[a]} list
 * @return {[a]} A copy of list without the first 'n' elements
 * @see R.take, R.transduce, R.dropLast, R.dropWhile
 * @example
 *
 *      R.drop(1, ['foo', 'bar', 'baz']); //=> ['bar', 'baz']
 *      R.drop(2, ['foo', 'bar', 'baz']); //=> ['baz']
 *      R.drop(3, ['foo', 'bar', 'baz']); //=> []
 *      R.drop(4, ['foo', 'bar', 'baz']); //=> []
 *      R.drop(3, 'ramda');               //=> 'da'
 */
module.exports = _curry2(_dispatchable(['drop'], _xdrop, function drop(n, xs) {
return slice(Math.max(0, n), Infinity, xs);
...
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
...
 * @sig Number -> String -> String
 * @param {Number} n The number of elements of 'list' to skip.
 * @param {Array} list The list of elements to consider.
 * @return {Array} A copy of the list with only the first 'list.length - n' elements
 * @see R.takeLast, R.drop, R.dropWhile, R.dropLastWhile
 * @example
 *
 *      R.dropLast(1, ['foo', 'bar', 'baz']); //=> ['foo', 'bar']
 *      R.dropLast(2, ['foo', 'bar', 'baz']); //=> ['foo']
 *      R.dropLast(3, ['foo', 'bar', 'baz']); //=> []
 *      R.dropLast(4, ['foo', 'bar', 'baz']); //=> []
 *      R.dropLast(3, 'ramda');               //=> 'ra'
 */
module.exports = _curry2(_dispatchable([], _xdropLast, _dropLast));
...
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
...
 * @param {Array} list The collection to iterate over.
 * @return {Array} A new array without any trailing elements that return 'falsy' values from the 'predicate'.
 * @see R.takeLastWhile, R.addIndex, R.drop, R.dropWhile
 * @example
 *
 *      var lteThree = x => x <= 3;
 *
 *      R.dropLastWhile(lteThree, [1, 2, 3, 4, 3, 2, 1]); //=> [1, 2, 3, 4]
 */
module.exports = _curry2(_dispatchable([], _xdropLastWhile, _dropLastWhile));
...
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
...
 * @category List
 * @sig [a] -> [a]
 * @param {Array} list The array to consider.
 * @return {Array} 'list' without repeating elements.
 * @see R.transduce
 * @example
 *
 *     R.dropRepeats([1, 1, 1, 2, 3, 4, 4, 2, 2]); //=> [1, 2, 3, 4, 2]
 */
module.exports = _curry1(_dispatchable([], _xdropRepeatsWith(equals), dropRepeatsWith(equals)));
...
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
...
 * @param {Function} pred A predicate used to test whether two items are equal.
 * @param {Array} list The array to consider.
 * @return {Array} 'list' without repeating elements.
 * @see R.transduce
 * @example
 *
 *      var l = [1, -1, 1, 3, 4, -4, -4, -5, 5, 3, 3];
 *      R.dropRepeatsWith(R.eqBy(Math.abs), l); //=> [1, 3, 4, -5, 3]
 */
module.exports = _curry2(_dispatchable([], _xdropRepeatsWith, function dropRepeatsWith(pred, list) {
var result = [];
var idx = 1;
var len = list.length;
if (len !== 0) {
  result[0] = list[0];
...
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
...
 * @param {Array} list The collection to iterate over.
 * @return {Array} A new array.
 * @see R.takeWhile, R.transduce, R.addIndex
 * @example
 *
 *      var lteTwo = x => x <= 2;
 *
 *      R.dropWhile(lteTwo, [1, 2, 3, 4, 3, 2, 1]); //=> [3, 4, 3, 2, 1]
 */
module.exports = _curry2(_dispatchable(['dropWhile'], _xdropWhile, function dropWhile(pred, list) {
var idx = 0;
var len = list.length;
while (idx < len && pred(list[idx])) {
  idx += 1;
}
...
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
...
 * @param {Function} g another predicate
 * @return {Function} a function that applies its arguments to 'f' and 'g' and '||'s their outputs together.
 * @see R.or
 * @example
 *
 *      var gt10 = x => x > 10;
 *      var even = x => x % 2 === 0;
 *      var f = R.either(gt10, even);
 *      f(101); //=> true
 *      f(8); //=> true
 */
module.exports = _curry2(function either(f, g) {
return _isFunction(f) ?
  function _either() {
    return f.apply(this, arguments) || g.apply(this, arguments);
...
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
...
 * @since v0.3.0
 * @category Function
 * @sig a -> a
 * @param {*} x
 * @return {*}
 * @example
 *
 *      R.empty(Just(42));      //=> Nothing()
 *      R.empty([1, 2, 3]);     //=> []
 *      R.empty('unicorns');    //=> ''
 *      R.empty({x: 1, y: 2});  //=> {}
 */
module.exports = _curry1(function empty(x) {
return (
  (x != null && typeof x.empty === 'function') ?
...
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
...
 * @param {Function} pred A predicate used to test whether two items are equal.
 * @param {Array} list The array to consider.
 * @return {Array} 'list' without repeating elements.
 * @see R.transduce
 * @example
 *
 *      var l = [1, -1, 1, 3, 4, -4, -4, -5, 5, 3, 3];
 *      R.dropRepeatsWith(R.eqBy(Math.abs), l); //=> [1, 3, 4, -5, 3]
 */
module.exports = _curry2(_dispatchable([], _xdropRepeatsWith, function dropRepeatsWith(pred, list) {
var result = [];
var idx = 1;
var len = list.length;
if (len !== 0) {
  result[0] = list[0];
...
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
...
 * @param {Object} obj2
 * @return {Boolean}
 *
 * @example
 *
 *      var o1 = { a: 1, b: 2, c: 3, d: 4 };
 *      var o2 = { a: 10, b: 20, c: 3, d: 40 };
 *      R.eqProps('a', o1, o2); //=> false
 *      R.eqProps('c', o1, o2); //=> true
 */
module.exports = _curry3(function eqProps(prop, obj1, obj2) {
  return equals(obj1[prop], obj2[prop]);
});
...
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
...
 * @param {Function} fn The predicate function.
 * @param {Array} list The array to consider.
 * @return {Boolean} 'true' if the predicate is satisfied by every element, 'false'
 *         otherwise.
 * @see R.any, R.none, R.transduce
 * @example
 *
 *      var equals3 = R.equals(3);
 *      R.all(equals3)([3, 3, 3, 3]); //=> true
 *      R.all(equals3)([3, 3, 1, 3]); //=> false
 */
module.exports = _curry2(_dispatchable(['all'], _xall, function all(fn, list) {
var idx = 0;
while (idx < list.length) {
  if (!fn(list[idx])) {
...
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
...
 *
 *      var tomato  = {firstName: '  Tomato ', data: {elapsed: 100, remaining: 1400}, id:123};
 *      var transformations = {
 *        firstName: R.trim,
 *        lastName: R.trim, // Will not get invoked.
 *        data: {elapsed: R.add(1), remaining: R.add(-1)}
 *      };
 *      R.evolve(transformations, tomato); //=> {firstName: 'Tomato', data: {elapsed: 101, remaining: 1399}, id:123}
 */
module.exports = _curry2(function evolve(transformations, object) {
var result = {};
var transformation, key, type;
for (key in object) {
  transformation = transformations[key];
  type = typeof transformation;
...
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
...
 * @param {Array} filterable
 * @return {Array}
 * @see R.reject, R.transduce, R.addIndex
 * @example
 *
 *      var isEven = n => n % 2 === 0;
 *
 *      R.filter(isEven, [1, 2, 3, 4]); //=> [2, 4]
 *
 *      R.filter(isEven, {a: 1, b: 2, c: 3, d: 4}); //=> {b: 2, d: 4}
 */
module.exports = _curry2(_dispatchable(['filter'], _xfilter, function(pred, filterable) {
return (
  _isObject(filterable) ?
    _reduce(function(acc, key) {
...
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
...
 *        desired one.
 * @param {Array} list The array to consider.
 * @return {Object} The element found, or 'undefined'.
 * @see R.transduce
 * @example
 *
 *      var xs = [{a: 1}, {a: 2}, {a: 3}];
 *      R.find(R.propEq('a', 2))(xs); //=> {a: 2}
 *      R.find(R.propEq('a', 4))(xs); //=> undefined
 */
module.exports = _curry2(_dispatchable(['find'], _xfind, function find(fn, list) {
var idx = 0;
var len = list.length;
while (idx < len) {
  if (fn(list[idx])) {
...
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
...
 * desired one.
 * @param {Array} list The array to consider.
 * @return {Number} The index of the element found, or '-1'.
 * @see R.transduce
 * @example
 *
 *      var xs = [{a: 1}, {a: 2}, {a: 3}];
 *      R.findIndex(R.propEq('a', 2))(xs); //=> 1
 *      R.findIndex(R.propEq('a', 4))(xs); //=> -1
 */
module.exports = _curry2(_dispatchable([], _xfindIndex, function findIndex(fn, list) {
var idx = 0;
var len = list.length;
while (idx < len) {
  if (fn(list[idx])) {
...
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
...
 * desired one.
 * @param {Array} list The array to consider.
 * @return {Object} The element found, or 'undefined'.
 * @see R.transduce
 * @example
 *
 *      var xs = [{a: 1, b: 0}, {a:1, b: 1}];
 *      R.findLast(R.propEq('a', 1))(xs); //=> {a: 1, b: 1}
 *      R.findLast(R.propEq('a', 4))(xs); //=> undefined
 */
module.exports = _curry2(_dispatchable([], _xfindLast, function findLast(fn, list) {
var idx = list.length - 1;
while (idx >= 0) {
  if (fn(list[idx])) {
    return list[idx];
...
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
...
 * desired one.
 * @param {Array} list The array to consider.
 * @return {Number} The index of the element found, or '-1'.
 * @see R.transduce
 * @example
 *
 *      var xs = [{a: 1, b: 0}, {a:1, b: 1}];
 *      R.findLastIndex(R.propEq('a', 1))(xs); //=> 1
 *      R.findLastIndex(R.propEq('a', 4))(xs); //=> -1
 */
module.exports = _curry2(_dispatchable([], _xfindLastIndex, function findLastIndex(fn, list) {
var idx = list.length - 1;
while (idx >= 0) {
  if (fn(list[idx])) {
    return idx;
...
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
...
 * @category List
 * @sig [a] -> [b]
 * @param {Array} list The array to consider.
 * @return {Array} The flattened list.
 * @see R.unnest
 * @example
 *
 *      R.flatten([1, 2, [3, 4], 5, [6, [7, 8, [9, [10, 11], 12]]]]);
 *      //=> [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
 */
module.exports = _curry1(_makeFlat(true));
...
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
...
 * @param {Function} fn The predicate function.
 * @param {Array} list The array to consider.
 * @return {Boolean} 'true' if the predicate is satisfied by at least one element, 'false'
 *         otherwise.
 * @see R.all, R.none, R.transduce
 * @example
 *
 *      var lessThan0 = R.flip(R.lt)(0);
 *      var lessThan2 = R.flip(R.lt)(2);
 *      R.any(lessThan0)([1, 2]); //=> false
 *      R.any(lessThan2)([1, 2]); //=> true
 */
module.exports = _curry2(_dispatchable(['any'], _xany, function any(fn, list) {
var idx = 0;
while (idx < list.length) {
...
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
...
 * @param {Function} fn The function to invoke. Receives one argument, 'value'.
 * @param {Array} list The list to iterate over.
 * @return {Array} The original list.
 * @see R.addIndex
 * @example
 *
 *      var printXPlusFive = x => console.log(x + 5);
 *      R.forEach(printXPlusFive, [1, 2, 3]); //=> [1, 2, 3]
 *      // logs 6
 *      // logs 7
 *      // logs 8
 * @symb R.forEach(f, [a, b, c]) = [a, b, c]
 */
module.exports = _curry2(_checkForMethod('forEach', function forEach(fn, list) {
var len = list.length;
...
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
...
 * @sig ((a, String, StrMap a) -> Any) -> StrMap a -> StrMap a
 * @param {Function} fn The function to invoke. Receives three argument, 'value', 'key', 'obj'.
 * @param {Object} obj The object to iterate over.
 * @return {Object} The original object.
 * @example
 *
 *      var printKeyConcatValue = (value, key) => console.log(key + ':' + value);
 *      R.forEachObjIndexed(printKeyConcatValue, {x: 1, y: 2}); //=> {x: 1, y: 2}
 *      // logs x:1
 *      // logs y:2
 * @symb R.forEachObjIndexed(f, {x: a, y: b}) = {x: a, y: b}
 */
module.exports = _curry2(function forEachObjIndexed(fn, obj) {
var keyList = keys(obj);
var idx = 0;
...
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
...
 * @category List
 * @sig [[k,v]] -> {k: v}
 * @param {Array} pairs An array of two-element arrays that will be the keys and values of the output object.
 * @return {Object} The object made by pairing up 'keys' and 'values'.
 * @see R.toPairs, R.pair
 * @example
 *
 *      R.fromPairs([['a', 1], ['b', 2], ['c', 3]]); //=> {a: 1, b: 2, c: 3}
 */
module.exports = _curry1(function fromPairs(pairs) {
var result = {};
var idx = 0;
while (idx < pairs.length) {
  result[pairs[idx][0]] = pairs[idx][1];
  idx += 1;
...
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
...
* @param {Function} fn Function :: a -> String
* @param {Array} list The array to group
* @return {Object} An object with the output of 'fn' for keys, mapped to arrays of elements
*         that produced that key when passed to 'fn'.
* @see R.transduce
* @example
*
*      var byGrade = R.groupBy(function(student) {
*        var score = student.score;
*        return score < 65 ? 'F' :
*               score < 70 ? 'D' :
*               score < 80 ? 'C' :
*               score < 90 ? 'B' : 'A';
*      });
*      var students = [{name: 'Abby', score: 84},
...
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
...
*        elements should be in the same group
* @param {Array} list The array to group. Also accepts a string, which will be
*        treated as a list of characters.
* @return {List} A list that contains sublists of equal elements,
*         whose concatenations are equal to the original list.
* @example
*
* R.groupWith(R.equals, [0, 1, 1, 2, 3, 5, 8, 13, 21])
* //=> [[0], [1, 1], [2], [3], [5], [8], [13], [21]]
*
* R.groupWith((a, b) => a % 2 === b % 2, [0, 1, 1, 2, 3, 5, 8, 13, 21])
* //=> [[0], [1, 1], [2], [3, 5], [8], [13, 21]]
*
* R.groupWith(R.eqBy(isVowel), 'aestiou')
* //=> ['ae', 'st', 'iou']
...
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
...
 * @sig (*... -> Boolean) -> (*... -> Boolean) -> (*... -> Boolean)
 * @param {Function} f A predicate
 * @param {Function} g Another predicate
 * @return {Function} a function that applies its arguments to 'f' and 'g' and '&&'s their outputs together.
 * @see R.and
 * @example
 *
 *      var gt10 = R.gt(R.__, 10)
 *      var lt20 = R.lt(R.__, 20)
 *      var f = R.both(gt10, lt20);
 *      f(15); //=> true
 *      f(30); //=> false
 */
module.exports = _curry2(function both(f, g) {
return _isFunction(f) ?
...
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
...
 * @sig Ord a => a -> a -> Boolean
 * @param {Number} a
 * @param {Number} b
 * @return {Boolean}
 * @see R.lte
 * @example
 *
 *      R.gte(2, 1); //=> true
 *      R.gte(2, 2); //=> true
 *      R.gte(2, 3); //=> false
 *      R.gte('a', 'z'); //=> false
 *      R.gte('z', 'a'); //=> true
 */
module.exports = _curry2(function gte(a, b) { return a >= b; });
...
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
...
* @category Object
* @sig s -> {s: x} -> Boolean
* @param {String} prop The name of the property to check for.
* @param {Object} obj The object to query.
* @return {Boolean} Whether the property exists.
* @example
*
*      var hasName = R.has('name');
*      hasName({name: 'alice'});   //=> true
*      hasName({name: 'bob'});     //=> true
*      hasName({});                //=> false
*
*      var point = {x: 0, y: 0};
*      var pointHas = R.has(R.__, point);
*      pointHas('x');  //=> true
...
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
...
 *        this.height = height;
 *      }
 *      Rectangle.prototype.area = function() {
 *        return this.width * this.height;
 *      };
 *
 *      var square = new Rectangle(2, 2);
 *      R.hasIn('width', square);  //=> true
 *      R.hasIn('area', square);  //=> true
 */
module.exports = _curry2(function hasIn(prop, obj) {
  return prop in obj;
});
...
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
...
 * @sig [a] -> a | Undefined
 * @sig String -> String
 * @param {Array|String} list
 * @return {*}
 * @see R.tail, R.init, R.last
 * @example
 *
 *      R.head(['fi', 'fo', 'fum']); //=> 'fi'
 *      R.head([]); //=> undefined
 *
 *      R.head('abc'); //=> 'a'
 *      R.head(''); //=> ''
 */
module.exports = nth(0);
...
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
...
 * @sig a -> a -> Boolean
 * @param {*} a
 * @param {*} b
 * @return {Boolean}
 * @example
 *
 *      var o = {};
 *      R.identical(o, o); //=> true
 *      R.identical(1, 1); //=> true
 *      R.identical(1, '1'); //=> false
 *      R.identical([], []); //=> false
 *      R.identical(0, -0); //=> false
 *      R.identical(NaN, NaN); //=> true
 */
module.exports = _curry2(function identical(a, b) {
...
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
...
 * @since v0.1.0
 * @category Function
 * @sig a -> a
 * @param {*} x The value to return.
 * @return {*} The input value, 'x'.
 * @example
 *
 *      R.identity(1); //=> 1
 *
 *      var obj = {};
 *      R.identity(obj) === obj; //=> true
 * @symb R.identity(a) = a
 */
module.exports = _curry1(_identity);
...
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
...
* @param {Function} onTrue A function to invoke when the 'condition' evaluates to a truthy value.
* @param {Function} onFalse A function to invoke when the 'condition' evaluates to a falsy value.
* @return {Function} A new unary function that will process either the 'onTrue' or the 'onFalse'
*                    function depending upon the result of the 'condition' predicate.
* @see R.unless, R.when
* @example
*
*      var incCount = R.ifElse(
*        R.has('count'),
*        R.over(R.lensProp('count'), R.inc),
*        R.assoc('count', 1)
*      );
*      incCount({});           //=> { count: 1 }
*      incCount({ count: 1 }); //=> { count: 2 }
*/
...
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
...
 * @category Math
 * @sig Number -> Number
 * @param {Number} n
 * @return {Number} n + 1
 * @see R.dec
 * @example
 *
 *      R.inc(42); //=> 43
 */
module.exports = add(1);
...
```

#### <a name="apidoc.element.ramda.indexBy"></a>[function <span class="apidocSignatureSpan">ramda.</span>indexBy (a0, a1)](#apidoc.element.ramda.indexBy)
- description and source-code
```javascript
indexBy = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
...
 * @sig (a -> String) -> [{k: v}] -> {k: {k: v}}
 * @param {Function} fn Function :: a -> String
 * @param {Array} array The array of objects to index
 * @return {Object} An object indexing each array element by the given property.
 * @example
 *
 *      var list = [{id: 'xyz', title: 'A'}, {id: 'abc', title: 'B'}];
 *      R.indexBy(R.prop('id'), list);
 *      //=> {abc: {id: 'abc', title: 'B'}, xyz: {id: 'xyz', title: 'A'}}
 */
module.exports = reduceBy(function(acc, elem) { return elem; }, null);
...
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
...
 * @sig a -> [a] -> Number
 * @param {*} target The item to find.
 * @param {Array} xs The array to search in.
 * @return {Number} the index of the target, or -1 if the target is not found.
 * @see R.lastIndexOf
 * @example
 *
 *      R.indexOf(3, [1,2,3,4]); //=> 2
 *      R.indexOf(10, [1,2,3,4]); //=> -1
 */
module.exports = _curry2(function indexOf(target, xs) {
  return typeof xs.indexOf === 'function' && !_isArray(xs) ?
    xs.indexOf(target) :
    _indexOf(xs, target, 0);
});
...
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
...
* @sig [a] -> [a]
* @sig String -> String
* @param {*} list
* @return {*}
* @see R.last, R.head, R.tail
* @example
*
*      R.init([1, 2, 3]);  //=> [1, 2]
*      R.init([1, 2]);     //=> [1]
*      R.init([1]);        //=> []
*      R.init([]);         //=> []
*
*      R.init('abc');  //=> 'ab'
*      R.init('ab');   //=> 'a'
*      R.init('a');    //=> ''
...
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
...
 * @sig Number -> a -> [a] -> [a]
 * @param {Number} index The position to insert the element
 * @param {*} elt The element to insert into the Array
 * @param {Array} list The list to insert into
 * @return {Array} A new Array with 'elt' inserted at 'index'.
 * @example
 *
 *      R.insert(2, 'x', [1,2,3,4]); //=> [1,2,'x',3,4]
 */
module.exports = _curry3(function insert(idx, elt, list) {
  idx = idx < list.length && idx >= 0 ? idx : list.length;
  var result = Array.prototype.slice.call(list, 0);
  result.splice(idx, 0, elt);
  return result;
});
...
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
...
 * @sig Number -> [a] -> [a] -> [a]
 * @param {Number} index The position to insert the sub-list
 * @param {Array} elts The sub-list to insert into the Array
 * @param {Array} list The list to insert the sub-list into
 * @return {Array} A new Array with 'elts' inserted starting at 'index'.
 * @example
 *
 *      R.insertAll(2, ['x','y','z'], [1,2,3,4]); //=> [1,2,'x','y','z',3,4]
 */
module.exports = _curry3(function insertAll(idx, elts, list) {
  idx = idx < list.length && idx >= 0 ? idx : list.length;
  return [].concat(Array.prototype.slice.call(list, 0, idx),
                   elts,
                   Array.prototype.slice.call(list, idx));
});
...
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
...
 * @sig [*] -> [*] -> [*]
 * @param {Array} list1 The first list.
 * @param {Array} list2 The second list.
 * @return {Array} The list of elements found in both 'list1' and 'list2'.
 * @see R.intersectionWith
 * @example
 *
 *      R.intersection([1,2,3,4], [7,6,5,4,3]); //=> [4, 3]
 */
module.exports = _curry2(function intersection(list1, list2) {
var lookupList, filteredList;
if (list1.length > list2.length) {
  lookupList = list1;
  filteredList = list2;
} else {
...
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
...
 *      var csny = [
 *        {id: 204, name: 'David Crosby'},
 *        {id: 456, name: 'Stephen Stills'},
 *        {id: 539, name: 'Graham Nash'},
 *        {id: 177, name: 'Neil Young'}
 *      ];
 *
 *      R.intersectionWith(R.eqBy(R.prop('id')), buffaloSpringfield, csny);
 *      //=> [{id: 456, name: 'Stephen Stills'}, {id: 177, name: 'Neil Young'}]
 */
module.exports = _curry3(function intersectionWith(pred, list1, list2) {
var lookupList, filteredList;
if (list1.length > list2.length) {
  lookupList = list1;
  filteredList = list2;
...
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
...
 * @category List
 * @sig a -> [a] -> [a]
 * @param {*} separator The element to add to the list.
 * @param {Array} list The list to be interposed.
 * @return {Array} The new list.
 * @example
 *
 *      R.intersperse('n', ['ba', 'a', 'a']); //=> ['ba', 'n', 'a', 'n', 'a']
 */
module.exports = _curry2(_checkForMethod('intersperse', function intersperse(separator, list) {
var out = [];
var idx = 0;
var length = list.length;
while (idx < length) {
  if (idx === length - 1) {
...
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
...
 * @param {Array} list The list to iterate over.
 * @return {*} The final, accumulated value.
 * @example
 *
 *      var numbers = [1, 2, 3, 4];
 *      var transducer = R.compose(R.map(R.add(1)), R.take(2));
 *
 *      R.into([], transducer, numbers); //=> [2, 3]
 *
 *      var intoArray = R.into([]);
 *      intoArray(transducer, numbers); //=> [2, 3]
 */
module.exports = _curry3(function into(acc, xf, list) {
return _isTransformer(acc) ?
  _reduce(xf(acc), acc['@@transducer/init'](), list) :
...
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
...
 * @example
 *
 *      var raceResultsByFirstName = {
 *        first: 'alice',
 *        second: 'jake',
 *        third: 'alice',
 *      };
 *      R.invert(raceResultsByFirstName);
 *      //=> { 'alice': ['first', 'third'], 'jake':['second'] }
 */
module.exports = _curry1(function invert(obj) {
var props = keys(obj);
var len = props.length;
var idx = 0;
var out = {};
...
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
...
* @return {Object} out A new object
* @example
*
*      var raceResults = {
*        first: 'alice',
*        second: 'jake'
*      };
*      R.invertObj(raceResults);
*      //=> { 'alice': 'first', 'jake':'second' }
*
*      // Alternatively:
*      var raceResults = ['alice', 'jake'];
*      R.invertObj(raceResults);
*      //=> { 'alice': '0', 'jake':'1' }
*/
...
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
...
 *
 *      var AnimalConstructor = R.construct(Animal)
 *
 *      // Notice we no longer need the 'new' keyword:
 *      AnimalConstructor('Pig'); //=> {"kind": "Pig", "sighting": function (){...}};
 *
 *      var animalTypes = ["Lion", "Tiger", "Bear"];
 *      var animalSighting = R.invoker(0, 'sighting');
 *      var sightNewAnimal = R.compose(animalSighting, AnimalConstructor);
 *      R.map(sightNewAnimal, animalTypes); //=> ["It's a Lion!", "It's a Tiger!", "It's a Bear!"]
 */
module.exports = _curry1(function construct(Fn) {
  return constructN(Fn.length, Fn);
});
...
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
...
* @category Type
* @sig (* -> {*}) -> a -> Boolean
* @param {Object} ctor A constructor
* @param {*} val The value to test
* @return {Boolean}
* @example
*
*      R.is(Object, {}); //=> true
*      R.is(Number, 1); //=> true
*      R.is(Object, 1); //=> false
*      R.is(String, 's'); //=> true
*      R.is(String, new String('')); //=> true
*      R.is(Object, new String('')); //=> true
*      R.is(Object, 's'); //=> false
*      R.is(Number, {}); //=> false
...
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
...
 * @category List
 * @sig * -> Boolean
 * @param {*} x The object to test.
 * @return {Boolean} 'true' if 'x' has a numeric length property and extreme indices defined; 'false' otherwise.
 * @deprecated since v0.23.0
 * @example
 *
 *      R.isArrayLike([]); //=> true
 *      R.isArrayLike(true); //=> false
 *      R.isArrayLike({}); //=> false
 *      R.isArrayLike({length: 10}); //=> false
 *      R.isArrayLike({0: 'zero', 9: 'nine', length: 10}); //=> true
 */
module.exports = _curry1(function isArrayLike(x) {
if (_isArray(x)) { return true; }
...
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
...
 * @category Logic
 * @sig a -> Boolean
 * @param {*} x
 * @return {Boolean}
 * @see R.empty
 * @example
 *
 *      R.isEmpty([1, 2, 3]);   //=> false
 *      R.isEmpty([]);          //=> true
 *      R.isEmpty('');          //=> true
 *      R.isEmpty(null);        //=> false
 *      R.isEmpty({});          //=> true
 *      R.isEmpty({length: 0}); //=> false
 */
module.exports = _curry1(function isEmpty(x) {
...
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
...
 * @since v0.9.0
 * @category Type
 * @sig * -> Boolean
 * @param {*} x The value to test.
 * @return {Boolean} 'true' if 'x' is 'undefined' or 'null', otherwise 'false'.
 * @example
 *
 *      R.isNil(null); //=> true
 *      R.isNil(undefined); //=> true
 *      R.isNil(0); //=> false
 *      R.isNil([]); //=> false
 */
module.exports = _curry1(function isNil(x) { return x == null; });
...
```

#### <a name="apidoc.element.ramda.join"></a>[function <span class="apidocSignatureSpan">ramda.</span>join (a0, a1)](#apidoc.element.ramda.join)
- description and source-code
```javascript
join = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
...
* @return {*}
* @see R.apply
* @example
*
*      R.call(R.add, 1, 2); //=> 3
*
*      var indentN = R.pipe(R.times(R.always(' ')),
*                           R.join(''),
*                           R.replace(/^(?!$)/gm));
*
*      var format = R.converge(R.call, [
*                                  R.pipe(R.prop('indent'), indentN),
*                                  R.prop('value')
*                              ]);
*
...
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
...
 * @category Function
 * @sig [(a, b, ..., m) -> n] -> ((a, b, ..., m) -> [n])
 * @param {Array} fns An array of functions
 * @return {Function} A function that returns a list of values after applying each of the original 'fns' to its parameters.
 * @see R.applySpec
 * @example
 *
 *      var getRange = R.juxt([Math.min, Math.max]);
 *      getRange(3, 4, 9, -3); //=> [-3, 9]
 * @symb R.juxt([f, g, h])(a, b) = [f(a, b), g(a, b), h(a, b)]
 */
module.exports = _curry1(function juxt(fns) {
  return converge(function() { return Array.prototype.slice.call(arguments, 0); }, fns);
});
...
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
...
 * @since v0.1.0
 * @category Object
 * @sig {k: v} -> [k]
 * @param {Object} obj The object to extract properties from
 * @return {Array} An array of the object's own properties.
 * @example
 *
 *      R.keys({a: 1, b: 2, c: 3}); //=> ['a', 'b', 'c']
 */
module.exports = (function() {
// cover IE < 9 keys issues
var hasEnumBug = !({toString: null}).propertyIsEnumerable('toString');
var nonEnumerableProps = ['constructor', 'valueOf', 'isPrototypeOf', 'toString',
                          'propertyIsEnumerable', 'hasOwnProperty', 'toLocaleString'];
// Safari bug
...
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
...
 * @param {Object} obj The object to extract properties from
 * @return {Array} An array of the object's own and prototype properties.
 * @example
 *
 *      var F = function() { this.x = 'X'; };
 *      F.prototype.y = 'Y';
 *      var f = new F();
 *      R.keysIn(f); //=> ['x', 'y']
 */
module.exports = _curry1(function keysIn(obj) {
var prop;
var ks = [];
for (prop in obj) {
  ks[ks.length] = prop;
}
...
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
...
 * @sig [a] -> a | Undefined
 * @sig String -> String
 * @param {*} list
 * @return {*}
 * @see R.init, R.head, R.tail
 * @example
 *
 *      R.last(['fi', 'fo', 'fum']); //=> 'fum'
 *      R.last([]); //=> undefined
 *
 *      R.last('abc'); //=> 'c'
 *      R.last(''); //=> ''
 */
module.exports = nth(-1);
...
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
...
 * @sig a -> [a] -> Number
 * @param {*} target The item to find.
 * @param {Array} xs The array to search in.
 * @return {Number} the index of the target, or -1 if the target is not found.
 * @see R.indexOf
 * @example
 *
 *      R.lastIndexOf(3, [-1,3,3,0,1,2,3,4]); //=> 6
 *      R.lastIndexOf(10, [1,2,3,4]); //=> -1
 */
module.exports = _curry2(function lastIndexOf(target, xs) {
if (typeof xs.lastIndexOf === 'function' && !_isArray(xs)) {
  return xs.lastIndexOf(target);
} else {
  var idx = xs.length - 1;
...
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
...
 * @since v0.3.0
 * @category List
 * @sig [a] -> Number
 * @param {Array} list The array to inspect.
 * @return {Number} The length of the array.
 * @example
 *
 *      R.length([]); //=> 0
 *      R.length([1, 2, 3]); //=> 3
 */
module.exports = _curry1(function length(list) {
  return list != null && _isNumber(list.length) ? list.length : NaN;
});
...
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
...
 * @sig (s -> a) -> ((a, s) -> s) -> Lens s a
 * @param {Function} getter
 * @param {Function} setter
 * @return {Lens}
 * @see R.view, R.set, R.over, R.lensIndex, R.lensProp
 * @example
 *
 *      var xLens = R.lens(R.prop('x'), R.assoc('x'));
 *
 *      R.view(xLens, {x: 1, y: 2});            //=> 1
 *      R.set(xLens, 4, {x: 1, y: 2});          //=> {x: 4, y: 2}
 *      R.over(xLens, R.negate, {x: 1, y: 2});  //=> {x: -1, y: 2}
 */
module.exports = _curry2(function lens(getter, setter) {
return function(toFunctorFn) {
...
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
...
 * @typedefn Lens s a = Functor f => (a -> f a) -> s -> f s
 * @sig Number -> Lens s a
 * @param {Number} n
 * @return {Lens}
 * @see R.view, R.set, R.over
 * @example
 *
 *      var headLens = R.lensIndex(0);
 *
 *      R.view(headLens, ['a', 'b', 'c']);            //=> 'a'
 *      R.set(headLens, 'x', ['a', 'b', 'c']);        //=> ['x', 'b', 'c']
 *      R.over(headLens, R.toUpper, ['a', 'b', 'c']); //=> ['A', 'b', 'c']
 */
module.exports = _curry1(function lensIndex(n) {
return lens(nth(n), update(n));
...
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
...
* @typedefn Lens s a = Functor f => (a -> f a) -> s -> f s
* @sig [Idx] -> Lens s a
* @param {Array} path The path to use.
* @return {Lens}
* @see R.view, R.set, R.over
* @example
*
*      var xHeadYLens = R.lensPath(['x', 0, 'y']);
*
*      R.view(xHeadYLens, {x: [{y: 2, z: 3}, {y: 4, z: 5}]});
*      //=> 2
*      R.set(xHeadYLens, 1, {x: [{y: 2, z: 3}, {y: 4, z: 5}]});
*      //=> {x: [{y: 1, z: 3}, {y: 4, z: 5}]}
*      R.over(xHeadYLens, R.negate, {x: [{y: 2, z: 3}, {y: 4, z: 5}]});
*      //=> {x: [{y: -2, z: 3}, {y: 4, z: 5}]}
...
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
...
 * @return {Function} A new unary function that will process either the 'onTrue' or the 'onFalse'
 *                    function depending upon the result of the 'condition' predicate.
 * @see R.unless, R.when
 * @example
 *
 *      var incCount = R.ifElse(
 *        R.has('count'),
 *        R.over(R.lensProp('count'), R.inc),
 *        R.assoc('count', 1)
 *      );
 *      incCount({});           //=> { count: 1 }
 *      incCount({ count: 1 }); //=> { count: 2 }
 */
module.exports = _curry3(function ifElse(condition, onTrue, onFalse) {
return curryN(Math.max(condition.length, onTrue.length, onFalse.length),
...
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
...
* @category Function
* @sig (*... -> *) -> ([*]... -> [*])
* @param {Function} fn The function to lift into higher context
* @return {Function} The lifted function.
* @see R.liftN
* @example
*
*      var madd3 = R.lift((a, b, c) => a + b + c);
*
*      madd3([1,2,3], [1,2,3], [1]); //=> [3, 4, 5, 4, 5, 6, 5, 6, 7]
*
*      var madd5 = R.lift((a, b, c, d, e) => a + b + c + d + e);
*
*      madd5([1,2], [3], [4, 5], [6], [7, 8]); //=> [21, 22, 22, 23, 22, 23, 23, 24]
*/
...
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
...
 * @category Function
 * @sig Number -> (*... -> *) -> ([*]... -> [*])
 * @param {Function} fn The function to lift into higher context
 * @return {Function} The lifted function.
 * @see R.lift, R.ap
 * @example
 *
 *      var madd3 = R.liftN(3, (...args) => R.sum(args));
 *      madd3([1,2,3], [1,2,3], [1]); //=> [3, 4, 5, 4, 5, 6, 5, 6, 7]
 */
module.exports = _curry2(function liftN(arity, fn) {
var lifted = curryN(arity, fn);
return curryN(arity, function() {
  return _reduce(ap, map(lifted, arguments[0]), Array.prototype.slice.call(arguments, 1));
});
...
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
...
 * @param {Function} f A predicate
 * @param {Function} g Another predicate
 * @return {Function} a function that applies its arguments to 'f' and 'g' and '&&'s their outputs together.
 * @see R.and
 * @example
 *
 *      var gt10 = R.gt(R.__, 10)
 *      var lt20 = R.lt(R.__, 20)
 *      var f = R.both(gt10, lt20);
 *      f(15); //=> true
 *      f(30); //=> false
 */
module.exports = _curry2(function both(f, g) {
return _isFunction(f) ?
  function _both() {
...
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
...
 * @sig Ord a => a -> a -> Boolean
 * @param {Number} a
 * @param {Number} b
 * @return {Boolean}
 * @see R.gte
 * @example
 *
 *      R.lte(2, 1); //=> false
 *      R.lte(2, 2); //=> true
 *      R.lte(2, 3); //=> true
 *      R.lte('a', 'z'); //=> true
 *      R.lte('z', 'a'); //=> false
 */
module.exports = _curry2(function lte(a, b) { return a <= b; });
...
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
...
 *
 *      // Notice we no longer need the 'new' keyword:
 *      AnimalConstructor('Pig'); //=> {"kind": "Pig", "sighting": function (){...}};
 *
 *      var animalTypes = ["Lion", "Tiger", "Bear"];
 *      var animalSighting = R.invoker(0, 'sighting');
 *      var sightNewAnimal = R.compose(animalSighting, AnimalConstructor);
 *      R.map(sightNewAnimal, animalTypes); //=> ["It's a Lion!", "It's a Tiger!", "It's a Bear!"]
 */
module.exports = _curry1(function construct(Fn) {
  return constructN(Fn.length, Fn);
});
...
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
...
* @return {*} The final, accumulated value.
* @see R.addIndex, R.mapAccumRight
* @example
*
*      var digits = ['1', '2', '3', '4'];
*      var appender = (a, b) => [a + b, a + b];
*
*      R.mapAccum(appender, 0, digits); //=> ['01234', ['01', '012', '0123', '01234']]
* @symb R.mapAccum(f, a, [b, c, d]) = [
*   f(f(f(a, b)[0], c)[0], d)[0],
*   [
*     f(a, b)[1],
*     f(f(a, b)[0], c)[1],
*     f(f(f(a, b)[0], c)[0], d)[1]
*   ]
...
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
...
* @return {*} The final, accumulated value.
* @see R.addIndex, R.mapAccum
* @example
*
*      var digits = ['1', '2', '3', '4'];
*      var append = (a, b) => [a + b, a + b];
*
*      R.mapAccumRight(append, 5, digits); //=> [['12345', '2345', '345', '45'], '12345']
* @symb R.mapAccumRight(f, a, [b, c, d]) = [
*   [
*     f(b, f(c, f(d, a)[0])[0])[1],
*     f(c, f(d, a)[0])[1],
*     f(d, a)[1],
*   ]
*   f(b, f(c, f(d, a)[0])[0])[0],
...
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
...
 * @return {Object}
 * @see R.map
 * @example
 *
 *      var values = { x: 1, y: 2, z: 3 };
 *      var prependKeyAndDouble = (num, key, obj) => key + (num * 2);
 *
 *      R.mapObjIndexed(prependKeyAndDouble, values); //=> { x: 'x2', y: 'y4', z: 'z6' }
 */
module.exports = _curry2(function mapObjIndexed(fn, obj) {
  return _reduce(function(acc, key) {
    acc[key] = fn(obj[key], key, obj);
    return acc;
  }, {}, keys(obj));
});
...
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
...
 * @sig RegExp -> String -> [String | Undefined]
 * @param {RegExp} rx A regular expression.
 * @param {String} str The string to match against
 * @return {Array} The list of matches or empty array.
 * @see R.test
 * @example
 *
 *      R.match(/([a-z]a)/g, 'bananas'); //=> ['ba', 'na', 'na']
 *      R.match(/a/, 'b'); //=> []
 *      R.match(/a/, null); //=> TypeError: null does not have a method named "match"
 */
module.exports = _curry2(function match(rx, str) {
  return str.match(rx) || [];
});
...
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
...
* @category Math
* @sig Number -> Number -> Number
* @param {Number} m The dividend.
* @param {Number} p the modulus.
* @return {Number} The result of 'b mod a'.
* @example
*
*      R.mathMod(-17, 5);  //=> 3
*      R.mathMod(17, 5);   //=> 2
*      R.mathMod(17, -5);  //=> NaN
*      R.mathMod(17, 0);   //=> NaN
*      R.mathMod(17.2, 5); //=> NaN
*      R.mathMod(17, 5.3); //=> NaN
*
*      var clock = R.mathMod(R.__, 12);
...
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
...
 *      R.drop(1, ['foo', 'bar', 'baz']); //=> ['bar', 'baz']
 *      R.drop(2, ['foo', 'bar', 'baz']); //=> ['baz']
 *      R.drop(3, ['foo', 'bar', 'baz']); //=> []
 *      R.drop(4, ['foo', 'bar', 'baz']); //=> []
 *      R.drop(3, 'ramda');               //=> 'da'
 */
module.exports = _curry2(_dispatchable(['drop'], _xdrop, function drop(n, xs) {
  return slice(Math.max(0, n), Infinity, xs);
}));
...
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
...
 * @return {*}
 * @see R.max, R.minBy
 * @example
 *
 *      //  square :: Number -> Number
 *      var square = n => n * n;
 *
 *      R.maxBy(square, -3, 2); //=> -3
 *
 *      R.reduce(R.maxBy(square), 0, [3, -5, 4, 1, -2]); //=> -5
 *      R.reduce(R.maxBy(square), 0, []); //=> 0
 */
module.exports = _curry3(function maxBy(f, a, b) {
  return f(b) > f(a) ? b : a;
});
...
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
...
 * @since v0.14.0
 * @category Math
 * @sig [Number] -> Number
 * @param {Array} list
 * @return {Number}
 * @example
 *
 *      R.mean([2, 7, 9]); //=> 6
 *      R.mean([]); //=> NaN
 */
module.exports = _curry1(function mean(list) {
  return sum(list) / list.length;
});
...
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
...
 * @since v0.14.0
 * @category Math
 * @sig [Number] -> Number
 * @param {Array} list
 * @return {Number}
 * @example
 *
 *      R.median([2, 9, 7]); //=> 7
 *      R.median([7, 2, 10, 9]); //=> 8
 *      R.median([]); //=> NaN
 */
module.exports = _curry1(function median(list) {
var len = list.length;
if (len === 0) {
  return NaN;
...
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
...
* @category Function
* @sig (*... -> a) -> (*... -> a)
* @param {Function} fn The function to memoize.
* @return {Function} Memoized version of 'fn'.
* @example
*
*      var count = 0;
*      var factorial = R.memoize(n => {
*        count += 1;
*        return R.product(R.range(1, n + 1));
*      });
*      factorial(5); //=> 120
*      factorial(5); //=> 120
*      factorial(5); //=> 120
*      count; //=> 1
...
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
...
 * @sig {k: v} -> {k: v} -> {k: v}
 * @param {Object} l
 * @param {Object} r
 * @return {Object}
 * @see R.mergeWith, R.mergeWithKey
 * @example
 *
 *      R.merge({ 'name': 'fred', 'age': 10 }, { 'age': 40 });
 *      //=> { 'name': 'fred', 'age': 40 }
 *
 *      var resetToDefault = R.merge(R.__, {x: 0});
 *      resetToDefault({x: 5, y: 2}); //=> {x: 0, y: 2}
 * @symb R.merge({ x: 1, y: 2 }, { y: 5, z: 3 }) = { x: 1, y: 5, z: 3 }
 */
module.exports = _curry2(function merge(l, r) {
...
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
...
 * @category List
 * @sig [{k: v}] -> {k: v}
 * @param {Array} list An array of objects
 * @return {Object} A merged object.
 * @see R.reduce
 * @example
 *
 *      R.mergeAll([{foo:1},{bar:2},{baz:3}]); //=> {foo:1,bar:2,baz:3}
 *      R.mergeAll([{foo:1},{foo:2},{bar:2}]); //=> {foo:2,bar:2}
 * @symb R.mergeAll([{ x: 1 }, { y: 2 }, { z: 3 }]) = { x: 1, y: 2, z: 3 }
 */
module.exports = _curry1(function mergeAll(list) {
  return _assign.apply(null, [{}].concat(list));
});
...
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
...
 * @param {Function} fn
 * @param {Object} l
 * @param {Object} r
 * @return {Object}
 * @see R.merge, R.mergeWithKey
 * @example
 *
 *      R.mergeWith(R.concat,
 *                  { a: true, values: [10, 20] },
 *                  { b: true, values: [15, 35] });
 *      //=> { a: true, b: true, values: [10, 20, 15, 35] }
 */
module.exports = _curry3(function mergeWith(fn, l, r) {
return mergeWithKey(function(_, _l, _r) {
  return fn(_l, _r);
...
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
...
 * @param {Object} l
 * @param {Object} r
 * @return {Object}
 * @see R.merge, R.mergeWith
 * @example
 *
 *      let concatValues = (k, l, r) => k == 'values' ? R.concat(l, r) : r
 *      R.mergeWithKey(concatValues,
 *                     { a: true, thing: 'foo', values: [10, 20] },
 *                     { b: true, thing: 'bar', values: [15, 35] });
 *      //=> { a: true, b: true, thing: 'bar', values: [10, 20, 15, 35] }
 * @symb R.mergeWithKey(f, { x: 1, y: 2 }, { y: 5, z: 3 }) = { x: 1, y: f('y', 2, 5), z: 3 }
 */
module.exports = _curry3(function mergeWithKey(fn, l, r) {
var result = {};
...
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
...
 *
 *      R.zip([1, 2, 3], ['a', 'b', 'c']); //=> [[1, 'a'], [2, 'b'], [3, 'c']]
 * @symb R.zip([a, b, c], [d, e, f]) = [[a, d], [b, e], [c, f]]
 */
module.exports = _curry2(function zip(a, b) {
  var rv = [];
  var idx = 0;
  var len = Math.min(a.length, b.length);
  while (idx < len) {
    rv[idx] = [a[idx], b[idx]];
    idx += 1;
  }
  return rv;
});
...
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
...
 * @return {*}
 * @see R.min, R.maxBy
 * @example
 *
 *      //  square :: Number -> Number
 *      var square = n => n * n;
 *
 *      R.minBy(square, -3, 2); //=> 2
 *
 *      R.reduce(R.minBy(square), Infinity, [3, -5, 4, 1, -2]); //=> 1
 *      R.reduce(R.minBy(square), Infinity, []); //=> Infinity
 */
module.exports = _curry3(function minBy(f, a, b) {
  return f(b) < f(a) ? b : a;
});
...
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
...
* @sig Number -> Number -> Number
* @param {Number} a The value to the divide.
* @param {Number} b The pseudo-modulus
* @return {Number} The result of 'b % a'.
* @see R.mathMod
* @example
*
*      R.modulo(17, 3); //=> 2
*      // JS behavior:
*      R.modulo(-17, 3); //=> -2
*      R.modulo(17, -3); //=> 2
*
*      var isOdd = R.modulo(R.__, 2);
*      isOdd(42); //=> 0
*      isOdd(21); //=> 1
...
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
...
 * @sig [a -> b] -> [a] -> [b]
 * @sig Apply f => f (a -> b) -> f a -> f b
 * @param {Array} fns An array of functions
 * @param {Array} vs An array of values
 * @return {Array} An array of results of applying each of 'fns' to all of 'vs' in turn.
 * @example
 *
 *      R.ap([R.multiply(2), R.add(3)], [1,2,3]); //=> [2, 4, 6, 4, 5, 6]
 *      R.ap([R.concat('tasty '), R.toUpper], ['pizza', 'salad']); //=> ["tasty pizza", "tasty salad", "PIZZA", "SALAD"]
 * @symb R.ap([f, g], [a, b]) = [f(a), f(b), g(a), g(b)]
 */
module.exports = _curry2(function ap(applicative, fn) {
return (
  typeof applicative.ap === 'function' ?
    applicative.ap(fn) :
...
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
...
* @example
*
*      var takesTwoArgs = (a, b) => [a, b];
*
*      takesTwoArgs.length; //=> 2
*      takesTwoArgs(1, 2); //=> [1, 2]
*
*      var takesOneArg = R.nAry(1, takesTwoArgs);
*      takesOneArg.length; //=> 1
*      // Only 'n' arguments are passed to the wrapped function
*      takesOneArg(1, 2); //=> [1, undefined]
* @symb R.nAry(0, f)(a, b) = f()
* @symb R.nAry(1, f)(a, b) = f(a)
* @symb R.nAry(2, f)(a, b) = f(a, b)
*/
...
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
...
 * @since v0.9.0
 * @category Math
 * @sig Number -> Number
 * @param {Number} n
 * @return {Number}
 * @example
 *
 *      R.negate(42); //=> -42
 */
module.exports = _curry1(function negate(n) { return -n; });
...
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
...
 * @param {Array} list The array to consider.
 * @return {Boolean} 'true' if the predicate is not satisfied by every element, 'false' otherwise.
 * @see R.all, R.any
 * @example
 *
 *      var isEven = n => n % 2 === 0;
 *
 *      R.none(isEven, [1, 3, 5, 7, 9, 11]); //=> true
 *      R.none(isEven, [1, 3, 5, 7, 8, 11]); //=> false
 */
module.exports = _curry2(_complement(_dispatchable(['any'], _xany, any)));
...
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
...
 * @category Logic
 * @sig * -> Boolean
 * @param {*} a any value
 * @return {Boolean} the logical inverse of passed argument.
 * @see R.complement
 * @example
 *
 *      R.not(true); //=> false
 *      R.not(false); //=> true
 *      R.not(0); //=> true
 *      R.not(1); //=> false
 */
module.exports = _curry1(function not(a) {
  return !a;
});
...
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
...
* @sig Number -> String -> String
* @param {Number} offset
* @param {*} list
* @return {*}
* @example
*
*      var list = ['foo', 'bar', 'baz', 'quux'];
*      R.nth(1, list); //=> 'bar'
*      R.nth(-1, list); //=> 'quux'
*      R.nth(-99, list); //=> undefined
*
*      R.nth(2, 'abc'); //=> 'c'
*      R.nth(3, 'abc'); //=> ''
* @symb R.nth(-1, [a, b, c]) = c
* @symb R.nth(0, [a, b, c]) = a
...
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
...
 * @since v0.9.0
 * @category Function
 * @sig Number -> *... -> *
 * @param {Number} n
 * @return {Function}
 * @example
 *
 *      R.nthArg(1)('a', 'b', 'c'); //=> 'b'
 *      R.nthArg(-1)('a', 'b', 'c'); //=> 'c'
 * @symb R.nthArg(-1)(a, b, c) = c
 * @symb R.nthArg(0)(a, b, c) = a
 * @symb R.nthArg(1)(a, b, c) = b
 */
module.exports = _curry1(function nthArg(n) {
var arity = n < 0 ? 1 : n + 1;
...
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
...
 * @param {String} key
 * @param {*} val
 * @return {Object}
 * @see R.pair
 * @example
 *
 *      var matchPhrases = R.compose(
 *        R.objOf('must'),
 *        R.map(R.objOf('match_phrase'))
 *      );
 *      matchPhrases(['foo', 'bar', 'baz']); //=> {must: [{match_phrase: 'foo'}, {match_phrase: 'bar'}, {match_phrase: 'baz'}]}
 */
module.exports = _curry2(function objOf(key, val) {
var obj = {};
obj[key] = val;
...
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
...
 * @since v0.3.0
 * @category Function
 * @sig a -> [a]
 * @param {*} x any value
 * @return {Array} An array wrapping 'x'.
 * @example
 *
 *      R.of(null); //=> [null]
 *      R.of([42]); //=> [[42]]
 */
module.exports = _curry1(_of);
...
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
...
 * @sig [String] -> {String: *} -> {String: *}
 * @param {Array} names an array of String property names to omit from the new object
 * @param {Object} obj The object to copy from
 * @return {Object} A new object with properties from 'names' not on it.
 * @see R.pick
 * @example
 *
 *      R.omit(['a', 'd'], {a: 1, b: 2, c: 3, d: 4}); //=> {b: 2, c: 3}
 */
module.exports = _curry2(function omit(names, obj) {
var result = {};
for (var prop in obj) {
  if (!_contains(prop, names)) {
    result[prop] = obj[prop];
  }
...
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
...
 * @since v0.1.0
 * @category Function
 * @sig (a... -> b) -> (a... -> b)
 * @param {Function} fn The function to wrap in a call-only-once wrapper.
 * @return {Function} The wrapped function.
 * @example
 *
 *      var addOneOnce = R.once(x => x + 1);
 *      addOneOnce(10); //=> 11
 *      addOneOnce(addOneOnce(50)); //=> 11
 */
module.exports = _curry1(function once(fn) {
var called = false;
var result;
return _arity(fn.length, function() {
...
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
...
 * @sig a -> b -> a | b
 * @param {Any} a
 * @param {Any} b
 * @return {Any} the first argument if truthy, otherwise the second argument.
 * @see R.either
 * @example
 *
 *      R.or(true, true); //=> true
 *      R.or(true, false); //=> true
 *      R.or(false, true); //=> true
 *      R.or(false, false); //=> false
 */
module.exports = _curry2(function or(a, b) {
  return a || b;
});
...
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
...
 * @return {Function} A new unary function that will process either the 'onTrue' or the 'onFalse'
 *                    function depending upon the result of the 'condition' predicate.
 * @see R.unless, R.when
 * @example
 *
 *      var incCount = R.ifElse(
 *        R.has('count'),
 *        R.over(R.lensProp('count'), R.inc),
 *        R.assoc('count', 1)
 *      );
 *      incCount({});           //=> { count: 1 }
 *      incCount({ count: 1 }); //=> { count: 2 }
 */
module.exports = _curry3(function ifElse(condition, onTrue, onFalse) {
return curryN(Math.max(condition.length, onTrue.length, onFalse.length),
...
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
...
 * @sig a -> b -> (a,b)
 * @param {*} fst
 * @param {*} snd
 * @return {Array}
 * @see R.objOf, R.of
 * @example
 *
 *      R.pair('foo', 'bar'); //=> ['foo', 'bar']
 */
module.exports = _curry2(function pair(fst, snd) { return [fst, snd]; });
...
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
...
* @param {Function} f
* @param {Array} args
* @return {Function}
* @see R.partialRight
* @example
*
*      var multiply2 = (a, b) => a * b;
*      var double = R.partial(multiply2, [2]);
*      double(2); //=> 4
*
*      var greet = (salutation, title, firstName, lastName) =>
*        salutation + ', ' + title + ' ' + firstName + ' ' + lastName + '!';
*
*      var sayHello = R.partial(greet, ['Hello']);
*      var sayHelloToMs = R.partial(sayHello, ['Ms.']);
...
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
...
 * @return {Function}
 * @see R.partial
 * @example
 *
 *      var greet = (salutation, title, firstName, lastName) =>
 *        salutation + ', ' + title + ' ' + firstName + ' ' + lastName + '!';
 *
 *      var greetMsJaneJones = R.partialRight(greet, ['Ms.', 'Jane', 'Jones']);
 *
 *      greetMsJaneJones('Hello'); //=> 'Hello, Ms. Jane Jones!'
 * @symb R.partialRight(f, [a, b])(c, d) = f(c, d, a, b)
 */
module.exports = _createPartialApplicator(flip(_concat));
...
```

#### <a name="apidoc.element.ramda.partition"></a>[function <span class="apidocSignatureSpan">ramda.</span>partition (a0, a1)](#apidoc.element.ramda.partition)
- description and source-code
```javascript
partition = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
...
 * @param {Function} pred A predicate to determine which side the element belongs to.
 * @param {Array} filterable the list (or other filterable) to partition.
 * @return {Array} An array, containing first the subset of elements that satisfy the
 *         predicate, and second the subset of elements that do not satisfy.
 * @see R.filter, R.reject
 * @example
 *
 *      R.partition(R.contains('s'), ['sss', 'ttt', 'foo', 'bars']);
 *      // => [ [ 'sss', 'bars' ],  [ 'ttt', 'foo' ] ]
 *
 *      R.partition(R.contains('s'), { a: 'sss', b: 'ttt', foo: 'bars' });
 *      // => [ { a: 'sss', foo: 'bars' }, { b: 'ttt' }  ]
 */
module.exports = juxt([filter, reject]);
...
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
...
 * @sig [Idx] -> {a} -> a | Undefined
 * @param {Array} path The path to use.
 * @param {Object} obj The object to retrieve the nested property from.
 * @return {*} The data at 'path'.
 * @see R.prop
 * @example
 *
 *      R.path(['a', 'b'], {a: {b: 2}}); //=> 2
 *      R.path(['a', 'b'], {c: {b: 2}}); //=> undefined
 */
module.exports = _curry2(function path(paths, obj) {
var val = obj;
var idx = 0;
while (idx < paths.length) {
  if (val == null) {
...
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
...
 *         'false' otherwise.
 * @example
 *
 *      var user1 = { address: { zipCode: 90210 } };
 *      var user2 = { address: { zipCode: 55555 } };
 *      var user3 = { name: 'Bob' };
 *      var users = [ user1, user2, user3 ];
 *      var isFamous = R.pathEq(['address', 'zipCode'], 90210);
 *      R.filter(isFamous, users); //=> [ user1 ]
 */
module.exports = _curry3(function pathEq(_path, val, obj) {
  return equals(path(_path, obj), val);
});
...
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
...
 * @sig a -> [Idx] -> {a} -> a
 * @param {*} d The default value.
 * @param {Array} p The path to use.
 * @param {Object} obj The object to retrieve the nested property from.
 * @return {*} The data at 'path' of the supplied object or the default value.
 * @example
 *
 *      R.pathOr('N/A', ['a', 'b'], {a: {b: 2}}); //=> 2
 *      R.pathOr('N/A', ['a', 'b'], {c: {b: 2}}); //=> "N/A"
 */
module.exports = _curry3(function pathOr(d, p, obj) {
  return defaultTo(d, path(p, obj));
});
...
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
...
 * @param {Function} pred
 * @param {Array} propPath
 * @param {*} obj
 * @return {Boolean}
 * @see R.propSatisfies, R.path
 * @example
 *
 *      R.pathSatisfies(y => y > 0, ['x', 'y'], {x: {y: 2}}); //=> true
 */
module.exports = _curry3(function pathSatisfies(pred, propPath, obj) {
  return propPath.length > 0 && pred(path(propPath, obj));
});
...
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
...
 * @sig [k] -> {k: v} -> {k: v}
 * @param {Array} names an array of String property names to copy onto a new object
 * @param {Object} obj The object to copy from
 * @return {Object} A new object with only properties from 'names' on it.
 * @see R.omit, R.props
 * @example
 *
 *      R.pick(['a', 'd'], {a: 1, b: 2, c: 3, d: 4}); //=> {a: 1, d: 4}
 *      R.pick(['a', 'e', 'f'], {a: 1, b: 2, c: 3, d: 4}); //=> {a: 1}
 */
module.exports = _curry2(function pick(names, obj) {
var result = {};
var idx = 0;
while (idx < names.length) {
  if (names[idx] in obj) {
...
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
...
 * @sig [k] -> {k: v} -> {k: v}
 * @param {Array} names an array of String property names to copy onto a new object
 * @param {Object} obj The object to copy from
 * @return {Object} A new object with only properties from 'names' on it.
 * @see R.pick
 * @example
 *
 *      R.pickAll(['a', 'd'], {a: 1, b: 2, c: 3, d: 4}); //=> {a: 1, d: 4}
 *      R.pickAll(['a', 'e', 'f'], {a: 1, b: 2, c: 3, d: 4}); //=> {a: 1, e: undefined, f: undefined}
 */
module.exports = _curry2(function pickAll(names, obj) {
var result = {};
var idx = 0;
var len = names.length;
while (idx < len) {
...
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
...
 * @param {Object} obj The object to copy from
 * @return {Object} A new object with only properties that satisfy 'pred'
 *         on it.
 * @see R.pick, R.filter
 * @example
 *
 *      var isUpperCase = (val, key) => key.toUpperCase() === key;
 *      R.pickBy(isUpperCase, {a: 1, b: 2, A: 3, B: 4}); //=> {A: 3, B: 4}
 */
module.exports = _curry2(function pickBy(test, obj) {
var result = {};
for (var prop in obj) {
  if (test(obj[prop], prop, obj)) {
    result[prop] = obj[prop];
  }
...
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
...
 * @param {Function} fn The function to bind to context
 * @param {Object} thisObj The context to bind 'fn' to
 * @return {Function} A function that will execute in the context of 'thisObj'.
 * @see R.partial
 * @example
 *
 *      var log = R.bind(console.log, console);
 *      R.pipe(R.assoc('a', 2), R.tap(log), R.assoc('a', 3))({a: 1}); //=> {a: 3}
 *      // logs {a: 2}
 * @symb R.bind(f, o)(a, b) = f.call(o, a, b)
 */
module.exports = _curry2(function bind(fn, thisObj) {
return _arity(fn.length, function() {
  return fn.apply(thisObj, arguments);
});
...
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
...
var composeK = require('./composeK');
var reverse = require('./reverse');

/**
* Returns the left-to-right Kleisli composition of the provided functions,
* each of which must return a value of a type supported by ['chain'](#chain).
*
* 'R.pipeK(f, g, h)' is equivalent to 'R.pipe(R.chain(f), R.chain(g), R.chain(h))'.
*
* @func
* @memberOf R
* @since v0.16.0
* @category Function
* @sig Chain m => ((a -> m b), (b -> m c), ..., (y -> m z)) -> (a -> m z)
* @param {...Function}
...
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
...
 * @sig ((a -> Promise b), (b -> Promise c), ..., (y -> Promise z)) -> (a -> Promise z)
 * @param {...Function} functions
 * @return {Function}
 * @see R.composeP
 * @example
 *
 *      //  followersForUser :: String -> Promise [User]
 *      var followersForUser = R.pipeP(db.getUserById, db.getFollowers);
 */
module.exports = function pipeP() {
if (arguments.length === 0) {
  throw new Error('pipeP requires at least one argument');
}
return _arity(arguments[0].length,
              reduce(_pipeP, arguments[0], tail(arguments)));
...
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
...
 * @sig k -> [{k: v}] -> [v]
 * @param {Number|String} key The key name to pluck off of each object.
 * @param {Array} list The array to consider.
 * @return {Array} The list of values for the given key.
 * @see R.props
 * @example
 *
 *      R.pluck('a')([{a: 1}, {a: 2}]); //=> [1, 2]
 *      R.pluck(0)([[1, 2], [3, 4]]);   //=> [1, 3]
 * @symb R.pluck('x', [{x: 1, y: 2}, {x: 3, y: 4}, {x: 5, y: 6}]) = [1, 3, 5]
 * @symb R.pluck(0, [[1, 2], [3, 4], [5, 6]]) = [1, 3, 5]
 */
module.exports = _curry2(function pluck(p, list) {
  return map(prop(p), list);
});
...
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
...
 * @sig a -> [a] -> [a]
 * @param {*} el The item to add to the head of the output list.
 * @param {Array} list The array to add to the tail of the output list.
 * @return {Array} A new array.
 * @see R.append
 * @example
 *
 *      R.prepend('fee', ['fi', 'fo', 'fum']); //=> ['fee', 'fi', 'fo', 'fum']
 */
module.exports = _curry2(function prepend(el, list) {
  return _concat([el], list);
});
...
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
...
 * @param {Function} fn The function to memoize.
 * @return {Function} Memoized version of 'fn'.
 * @example
 *
 *      var count = 0;
 *      var factorial = R.memoize(n => {
 *        count += 1;
 *        return R.product(R.range(1, n + 1));
 *      });
 *      factorial(5); //=> 120
 *      factorial(5); //=> 120
 *      factorial(5); //=> 120
 *      count; //=> 1
 */
module.exports = _curry1(function memoize(fn) {
...
```

#### <a name="apidoc.element.ramda.project"></a>[function <span class="apidocSignatureSpan">ramda.</span>project (a0, a1)](#apidoc.element.ramda.project)
- description and source-code
```javascript
project = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
...
 * @param {Array} objs The objects to query
 * @return {Array} An array of objects with just the 'props' properties.
 * @example
 *
 *      var abby = {name: 'Abby', age: 7, hair: 'blond', grade: 2};
 *      var fred = {name: 'Fred', age: 12, hair: 'brown', grade: 7};
 *      var kids = [abby, fred];
 *      R.project(['name', 'grade'], kids); //=> [{name: 'Abby', grade: 2}, {name: 'Fred', grade: 7}]
 */
module.exports = useWith(_map, [pickAll, identity]); // passing 'identity' gives correct arity
...
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
...
 * @sig Ord b => (a -> b) -> a -> a -> Number
 * @param {Function} fn A function of arity one that returns a value that can be compared
 * @param {*} a The first item to be compared.
 * @param {*} b The second item to be compared.
 * @return {Number} '-1' if fn(a) < fn(b), '1' if fn(b) < fn(a), otherwise '0'
 * @example
 *
 *      var byAge = R.ascend(R.prop('age'));
 *      var people = [
 *        // ...
 *      ];
 *      var peopleByYoungestFirst = R.sort(byAge, people);
 */
module.exports = _curry3(function ascend(fn, a, b) {
var aa = fn(a);
...
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
...
 * @category Logic
 * @sig [(*... -> Boolean)] -> (*... -> Boolean)
 * @param {Array} predicates An array of predicates to check
 * @return {Function} The combined predicate
 * @see R.anyPass
 * @example
 *
 *      var isQueen = R.propEq('rank', 'Q');
 *      var isSpade = R.propEq('suit', '♠︎');
 *      var isQueenOfSpades = R.allPass([isQueen, isSpade]);
 *
 *      isQueenOfSpades({rank: 'Q', suit: '♣︎'}); //=> false
 *      isQueenOfSpades({rank: 'Q', suit: '♠︎'}); //=> true
 */
module.exports = _curry1(function allPass(preds) {
...
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
...
 * @param {Function} type
 * @param {String} name
 * @param {*} obj
 * @return {Boolean}
 * @see R.is, R.propSatisfies
 * @example
 *
 *      R.propIs(Number, 'x', {x: 1, y: 2});  //=> true
 *      R.propIs(Number, 'x', {x: 'foo'});    //=> false
 *      R.propIs(Number, 'x', {});            //=> false
 */
module.exports = _curry3(function propIs(type, name, obj) {
  return is(type, obj[name]);
});
...
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
...
 * @example
 *
 *      var alice = {
 *        name: 'ALICE',
 *        age: 101
 *      };
 *      var favorite = R.prop('favoriteLibrary');
 *      var favoriteWithDefault = R.propOr('Ramda', 'favoriteLibrary');
 *
 *      favorite(alice);  //=> undefined
 *      favoriteWithDefault(alice);  //=> 'Ramda'
 */
module.exports = _curry3(function propOr(val, p, obj) {
  return (obj != null && _has(p, obj)) ? obj[p] : val;
});
...
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
...
 * @param {Function} pred
 * @param {String} name
 * @param {*} obj
 * @return {Boolean}
 * @see R.propEq, R.propIs
 * @example
 *
 *      R.propSatisfies(x => x > 0, 'x', {x: 1, y: 2}); //=> true
 */
module.exports = _curry3(function propSatisfies(pred, name, obj) {
  return pred(obj[name]);
});
...
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
...
 * @category Object
 * @sig [k] -> {k: v} -> [v]
 * @param {Array} ps The property names to fetch
 * @param {Object} obj The object to query
 * @return {Array} The corresponding values or partially applied function.
 * @example
 *
 *      R.props(['x', 'y'], {x: 1, y: 2}); //=> [1, 2]
 *      R.props(['c', 'a', 'b'], {b: 2, a: 1}); //=> [undefined, 1, 2]
 *
 *      var fullName = R.compose(R.join(' '), R.props(['first', 'last']));
 *      fullName({last: 'Bullet-Tooth', age: 33, first: 'Tony'}); //=> 'Tony Bullet-Tooth'
 */
module.exports = _curry2(function props(ps, obj) {
var len = ps.length;
...
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
...
 * @param {Function} fn The function to memoize.
 * @return {Function} Memoized version of 'fn'.
 * @example
 *
 *      var count = 0;
 *      var factorial = R.memoize(n => {
 *        count += 1;
 *        return R.product(R.range(1, n + 1));
 *      });
 *      factorial(5); //=> 120
 *      factorial(5); //=> 120
 *      factorial(5); //=> 120
 *      count; //=> 1
 */
module.exports = _curry1(function memoize(fn) {
...
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
...
 * @example
 *
 *      //  square :: Number -> Number
 *      var square = n => n * n;
 *
 *      R.maxBy(square, -3, 2); //=> -3
 *
 *      R.reduce(R.maxBy(square), 0, [3, -5, 4, 1, -2]); //=> -5
 *      R.reduce(R.maxBy(square), 0, []); //=> 0
 */
module.exports = _curry3(function maxBy(f, a, b) {
  return f(b) > f(a) ? b : a;
});
...
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
...
* @param {Function} keyFn The function that maps the list's element into a key.
* @param {Array} list The array to group.
* @return {Object} An object with the output of 'keyFn' for keys, mapped to the output of
*         'valueFn' for elements which produced that key when passed to 'keyFn'.
* @see R.groupBy, R.reduce
* @example
*
*      var reduceToNamesBy = R.reduceBy((acc, student) => acc.concat(student.name), []);
*      var namesByGrade = reduceToNamesBy(function(student) {
*        var score = student.score;
*        return score < 65 ? 'F' :
*               score < 70 ? 'D' :
*               score < 80 ? 'C' :
*               score < 90 ? 'B' : 'A';
*      });
...
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
...
*        and the accumulator.
* @param {*} acc The accumulator value.
* @param {Array} list The list to iterate over.
* @return {*} The final, accumulated value.
* @see R.reduce, R.addIndex
* @example
*
*      R.reduceRight(R.subtract, 0, [1, 2, 3, 4]) // => (1 - (2 - (3 - (4 - 0)))) = -2
*          -               -2
*         / \              / \
*        1   -            1   3
*           / \              / \
*          2   -     ==>    2  -1
*             / \              / \
*            3   -            3   4
...
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
...
 * @param {Array} list The list to iterate over.
 * @return {*} The final, accumulated value.
 * @see R.reduce, R.reduced
 * @example
 *
 *      var isOdd = (acc, x) => x % 2 === 1;
 *      var xs = [1, 3, 5, 60, 777, 800];
 *      R.reduceWhile(isOdd, R.add, 0, xs); //=> 9
 *
 *      var ys = [2, 4, 6]
 *      R.reduceWhile(isOdd, R.add, 111, ys); //=> 111
 */
module.exports = _curryN(4, [], function _reduceWhile(pred, fn, a, list) {
return _reduce(function(acc, x) {
  return pred(acc, x) ? fn(acc, x) : _reduced(acc);
...
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
...
 * @param {Array} filterable
 * @return {Array}
 * @see R.filter, R.transduce, R.addIndex
 * @example
 *
 *      var isOdd = (n) => n % 2 === 1;
 *
 *      R.reject(isOdd, [1, 2, 3, 4]); //=> [2, 4]
 *
 *      R.reject(isOdd, {a: 1, b: 2, c: 3, d: 4}); //=> {b: 2, d: 4}
 */
module.exports = _curry2(function reject(pred, filterable) {
  return filter(_complement(pred), filterable);
});
...
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
...
 * @sig Number -> Number -> [a] -> [a]
 * @param {Number} start The position to start removing elements
 * @param {Number} count The number of elements to remove
 * @param {Array} list The list to remove from
 * @return {Array} A new Array with 'count' elements from 'start' removed.
 * @example
 *
 *      R.remove(2, 3, [1,2,3,4,5,6,7,8]); //=> [1,2,6,7,8]
 */
module.exports = _curry3(function remove(start, count, list) {
  var result = Array.prototype.slice.call(list, 0);
  result.splice(start, count);
  return result;
});
...
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
...
* @category List
* @sig a -> n -> [a]
* @param {*} value The value to repeat.
* @param {Number} n The desired size of the output list.
* @return {Array} A new array containing 'n' 'value's.
* @example
*
*      R.repeat('hi', 5); //=> ['hi', 'hi', 'hi', 'hi', 'hi']
*
*      var obj = {};
*      var repeatedObjs = R.repeat(obj, 5); //=> [{}, {}, {}, {}, {}]
*      repeatedObjs[0] === repeatedObjs[1]; //=> true
* @symb R.repeat(a, 0) = []
* @symb R.repeat(a, 1) = [a]
* @symb R.repeat(a, 2) = [a, a]
...
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
...
 *
 * @constant
 * @memberOf R
 * @since v0.6.0
 * @category Function
 * @example
 *
 *      var greet = R.replace('{name}', R.__, 'Hello, {name}!');
 *      greet('Alice'); //=> 'Hello, Alice!'
 */
module.exports = {'@@functional/placeholder': true};
...
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
...
* @category List
* @sig [a] -> [a]
* @sig String -> String
* @param {Array|String} list
* @return {Array|String}
* @example
*
*      R.reverse([1, 2, 3]);  //=> [3, 2, 1]
*      R.reverse([1, 2]);     //=> [2, 1]
*      R.reverse([1]);        //=> [1]
*      R.reverse([]);         //=> []
*
*      R.reverse('abc');      //=> 'cba'
*      R.reverse('ab');       //=> 'ba'
*      R.reverse('a');        //=> 'a'
...
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
...
 *        current element from the array
 * @param {*} acc The accumulator value.
 * @param {Array} list The list to iterate over.
 * @return {Array} A list of all intermediately reduced values.
 * @example
 *
 *      var numbers = [1, 2, 3, 4];
 *      var factorials = R.scan(R.multiply, 1, numbers); //=> [1, 1, 2, 6, 24]
 * @symb R.scan(f, a, [b, c]) = [a, f(a, b), f(f(a, b), c)]
 */
module.exports = _curry3(function scan(fn, acc, list) {
var idx = 0;
var len = list.length;
var result = [acc];
while (idx < len) {
...
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
...
 * @sig (Applicative f, Traversable t) => (a -> f a) -> t (f a) -> f (t a)
 * @param {Function} of
 * @param {*} traversable
 * @return {*}
 * @see R.traverse
 * @example
 *
 *      R.sequence(Maybe.of, [Just(1), Just(2), Just(3)]);   //=> Just([1, 2, 3])
 *      R.sequence(Maybe.of, [Just(1), Just(2), Nothing()]); //=> Nothing()
 *
 *      R.sequence(R.of, Just([1, 2, 3])); //=> [Just(1), Just(2), Just(3)]
 *      R.sequence(R.of, Nothing());       //=> [Nothing()]
 */
module.exports = _curry2(function sequence(of, traversable) {
return typeof traversable.sequence === 'function' ?
...
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
...
 * @return {Lens}
 * @see R.view, R.set, R.over, R.lensIndex, R.lensProp
 * @example
 *
 *      var xLens = R.lens(R.prop('x'), R.assoc('x'));
 *
 *      R.view(xLens, {x: 1, y: 2});            //=> 1
 *      R.set(xLens, 4, {x: 1, y: 2});          //=> {x: 4, y: 2}
 *      R.over(xLens, R.negate, {x: 1, y: 2});  //=> {x: -1, y: 2}
 */
module.exports = _curry2(function lens(getter, setter) {
return function(toFunctorFn) {
  return function(target) {
    return map(
      function(focus) {
...
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
...
  var idx = 0;
  var len = list.length;
  while (idx < len) {
    var nextidx = idx + 1;
    while (nextidx < len && fn(list[idx], list[nextidx])) {
      nextidx += 1;
    }
    res.push(list.slice(idx, nextidx));
    idx = nextidx;
  }
  return res;
});
...
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
...
 * @return {Number} '-1' if fn(a) < fn(b), '1' if fn(b) < fn(a), otherwise '0'
 * @example
 *
 *      var byAge = R.ascend(R.prop('age'));
 *      var people = [
 *        // ...
 *      ];
 *      var peopleByYoungestFirst = R.sort(byAge, people);
 */
module.exports = _curry3(function ascend(fn, a, b) {
  var aa = fn(a);
  var bb = fn(b);
  return aa < bb ? -1 : aa > bb ? 1 : 0;
});
...
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
...
* @category Relation
* @sig Ord b => (a -> b) -> [a] -> [a]
* @param {Function} fn
* @param {Array} list The list to sort.
* @return {Array} A new list sorted by the keys generated by 'fn'.
* @example
*
*      var sortByFirstItem = R.sortBy(R.prop(0));
*      var sortByNameCaseInsensitive = R.sortBy(R.compose(R.toLower, R.prop('name')));
*      var pairs = [[-1, 1], [-2, 2], [-3, 3]];
*      sortByFirstItem(pairs); //=> [[-3, 3], [-2, 2], [-1, 1]]
*      var alice = {
*        name: 'ALICE',
*        age: 101
*      };
...
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
...
 *        age: 30
 *      };
 *      var clara = {
 *        name: 'clara',
 *        age: 40
 *      };
 *      var people = [clara, bob, alice];
 *      var ageNameSort = R.sortWith([
 *        R.descend(R.prop('age')),
 *        R.ascend(R.prop('name'))
 *      ]);
 *      ageNameSort(people); //=> [alice, clara, bob]
 */
module.exports = _curry2(function sortWith(fns, list) {
return Array.prototype.slice.call(list, 0).sort(function(a, b) {
...
```

#### <a name="apidoc.element.ramda.split"></a>[function <span class="apidocSignatureSpan">ramda.</span>split (a0, a1)](#apidoc.element.ramda.split)
- description and source-code
```javascript
split = function (a0, a1) { return fn.apply(this, arguments); }
```
- example usage
```shell
...
 *
 *      R.reverse('abc');      //=> 'cba'
 *      R.reverse('ab');       //=> 'ba'
 *      R.reverse('a');        //=> 'a'
 *      R.reverse('');         //=> ''
 */
module.exports = _curry1(function reverse(list) {
  return _isString(list) ? list.split('').reverse().join('') :
                           Array.prototype.slice.call(list, 0).reverse();
});
...
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
...
 * @sig Number -> [a] -> [[a], [a]]
 * @sig Number -> String -> [String, String]
 * @param {Number} index The index where the array/string is split.
 * @param {Array|String} array The array/string to be split.
 * @return {Array}
 * @example
 *
 *      R.splitAt(1, [1, 2, 3]);          //=> [[1], [2, 3]]
 *      R.splitAt(5, 'hello world');      //=> ['hello', ' world']
 *      R.splitAt(-1, 'foobar');          //=> ['fooba', 'r']
 */
module.exports = _curry2(function splitAt(index, array) {
  return [slice(0, index, array), slice(index, length(array), array)];
});
...
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
...
 * @sig Number -> [a] -> [[a]]
 * @sig Number -> String -> [String]
 * @param {Number} n
 * @param {Array} list
 * @return {Array}
 * @example
 *
 *      R.splitEvery(3, [1, 2, 3, 4, 5, 6, 7]); //=> [[1, 2, 3], [4, 5, 6], [7]]
 *      R.splitEvery(3, 'foobarbaz'); //=> ['foo', 'bar', 'baz']
 */
module.exports = _curry2(function splitEvery(n, list) {
if (n <= 0) {
  throw new Error('First argument to splitEvery must be a positive integer');
}
var result = [];
...
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
...
 * @category List
 * @sig (a -> Boolean) -> [a] -> [[a], [a]]
 * @param {Function} pred The predicate that determines where the array is split.
 * @param {Array} list The array to be split.
 * @return {Array}
 * @example
 *
 *      R.splitWhen(R.equals(2), [1, 2, 3, 1, 2, 3]);   //=> [[1], [2, 3, 1, 2, 3]]
 */
module.exports = _curry2(function splitWhen(pred, list) {
var idx = 0;
var len = list.length;
var prefix = [];

while (idx < len && !pred(list[idx])) {
...
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
...
* @sig Number -> Number -> Number
* @param {Number} a The first value.
* @param {Number} b The second value.
* @return {Number} The result of 'a - b'.
* @see R.add
* @example
*
*      R.subtract(10, 8); //=> 2
*
*      var minus5 = R.subtract(R.__, 5);
*      minus5(17); //=> 12
*
*      var complementaryAngle = R.subtract(90);
*      complementaryAngle(30); //=> 60
*      complementaryAngle(72); //=> 18
...
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
...
 * @sig Number -> (* -> a) -> (* -> a)
 * @param {Number} length The arity for the returned function.
 * @param {Function} fn The function to curry.
 * @return {Function} A new, curried function.
 * @see R.curry
 * @example
 *
 *      var sumArgs = (...args) => R.sum(args);
 *
 *      var curriedAddFourNumbers = R.curryN(4, sumArgs);
 *      var f = curriedAddFourNumbers(1, 2);
 *      var g = f(3);
 *      g(4); //=> 10
 */
module.exports = _curry2(function curryN(length, fn) {
...
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
...
 * @sig [*] -> [*] -> [*]
 * @param {Array} list1 The first list.
 * @param {Array} list2 The second list.
 * @return {Array} The elements in 'list1' or 'list2', but not both.
 * @see R.symmetricDifferenceWith, R.difference, R.differenceWith
 * @example
 *
 *      R.symmetricDifference([1,2,3,4], [7,6,5,4,3]); //=> [1,2,7,6,5]
 *      R.symmetricDifference([7,6,5,4,3], [1,2,3,4]); //=> [7,6,5,1,2]
 */
module.exports = _curry2(function symmetricDifference(list1, list2) {
  return concat(difference(list1, list2), difference(list2, list1));
});
...
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
...
 * @return {Array} The elements in 'list1' or 'list2', but not both.
 * @see R.symmetricDifference, R.difference, R.differenceWith
 * @example
 *
 *      var eqA = R.eqBy(R.prop('a'));
 *      var l1 = [{a: 1}, {a: 2}, {a: 3}, {a: 4}];
 *      var l2 = [{a: 3}, {a: 4}, {a: 5}, {a: 6}];
 *      R.symmetricDifferenceWith(eqA, l1, l2); //=> [{a: 1}, {a: 2}, {a: 5}, {a: 6}]
 */
module.exports = _curry3(function symmetricDifferenceWith(pred, list1, list2) {
  return concat(differenceWith(pred, list1, list2), differenceWith(pred, list2, list1));
});
...
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
...
 * @param {String|RegExp} sep The pattern.
 * @param {String} str The string to separate into an array.
 * @return {Array} The array of strings from 'str' separated by 'str'.
 * @see R.join
 * @example
 *
 *      var pathComponents = R.split('/');
 *      R.tail(pathComponents('/usr/local/bin/node')); //=> ['usr', 'local', 'bin', 'node']
 *
 *      R.split('.', 'a.b.c.xyz.d'); //=> ['a', 'b', 'c', 'xyz', 'd']
 */
module.exports = invoker(1, 'split');
...
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
...
 * @param {*} acc The initial accumulator value.
 * @param {Function} xf The transducer function. Receives a transformer and returns a transformer.
 * @param {Array} list The list to iterate over.
 * @return {*} The final, accumulated value.
 * @example
 *
 *      var numbers = [1, 2, 3, 4];
 *      var transducer = R.compose(R.map(R.add(1)), R.take(2));
 *
 *      R.into([], transducer, numbers); //=> [2, 3]
 *
 *      var intoArray = R.into([]);
 *      intoArray(transducer, numbers); //=> [2, 3]
 */
module.exports = _curry3(function into(acc, xf, list) {
...
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
...
 * @sig Number -> String -> String
 * @param {Number} n The number of elements to return.
 * @param {Array} xs The collection to consider.
 * @return {Array}
 * @see R.dropLast
 * @example
 *
 *      R.takeLast(1, ['foo', 'bar', 'baz']); //=> ['baz']
 *      R.takeLast(2, ['foo', 'bar', 'baz']); //=> ['bar', 'baz']
 *      R.takeLast(3, ['foo', 'bar', 'baz']); //=> ['foo', 'bar', 'baz']
 *      R.takeLast(4, ['foo', 'bar', 'baz']); //=> ['foo', 'bar', 'baz']
 *      R.takeLast(3, 'ramda');               //=> 'mda'
 */
module.exports = _curry2(function takeLast(n, xs) {
return drop(n >= 0 ? xs.length - n : 0, xs);
...
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
...
 * @param {Array} list The collection to iterate over.
 * @return {Array} A new array.
 * @see R.dropLastWhile, R.addIndex
 * @example
 *
 *      var isNotOne = x => x !== 1;
 *
 *      R.takeLastWhile(isNotOne, [1, 2, 3, 4]); //=> [2, 3, 4]
 */
module.exports = _curry2(function takeLastWhile(fn, list) {
var idx = list.length - 1;
while (idx >= 0 && fn(list[idx])) {
  idx -= 1;
}
return Array.prototype.slice.call(list, idx + 1);
...
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
...
 * @param {Array} list The collection to iterate over.
 * @return {Array} A new array.
 * @see R.dropWhile, R.transduce, R.addIndex
 * @example
 *
 *      var isNotFour = x => x !== 4;
 *
 *      R.takeWhile(isNotFour, [1, 2, 3, 4, 3, 2, 1]); //=> [1, 2, 3]
 */
module.exports = _curry2(_dispatchable(['takeWhile'], _xtakeWhile, function takeWhile(fn, list) {
var idx = 0;
var len = list.length;
while (idx < len && fn(list[idx])) {
  idx += 1;
}
...
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
...
 * @param {Function} fn The function to bind to context
 * @param {Object} thisObj The context to bind 'fn' to
 * @return {Function} A function that will execute in the context of 'thisObj'.
 * @see R.partial
 * @example
 *
 *      var log = R.bind(console.log, console);
 *      R.pipe(R.assoc('a', 2), R.tap(log), R.assoc('a', 3))({a: 1}); //=> {a: 3}
 *      // logs {a: 2}
 * @symb R.bind(f, o)(a, b) = f.call(o, a, b)
 */
module.exports = _curry2(function bind(fn, thisObj) {
return _arity(fn.length, function() {
  return fn.apply(thisObj, arguments);
});
...
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
...
* @param {...*} args Any number of positional arguments.
* @return {*}
* @see R.apply
* @example
*
*      R.call(R.add, 1, 2); //=> 3
*
*      var indentN = R.pipe(R.times(R.always(' ')),
*                           R.join(''),
*                           R.replace(/^(?!$)/gm));
*
*      var format = R.converge(R.call, [
*                                  R.pipe(R.prop('indent'), indentN),
*                                  R.prop('value')
*                              ]);
...
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
...
 * @category String
 * @sig String -> String
 * @param {String} str The string to lower case.
 * @return {String} The lower case version of 'str'.
 * @see R.toUpper
 * @example
 *
 *      R.toLower('XYZ'); //=> 'xyz'
 */
module.exports = invoker(0, 'toLowerCase');
...
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
...
 * @category Object
 * @sig {String: *} -> [[String,*]]
 * @param {Object} obj The object to extract from
 * @return {Array} An array of key, value arrays from the object's own properties.
 * @see R.fromPairs
 * @example
 *
 *      R.toPairs({a: 1, b: 2, c: 3}); //=> [['a', 1], ['b', 2], ['c', 3]]
 */
module.exports = _curry1(function toPairs(obj) {
var pairs = [];
for (var prop in obj) {
  if (_has(prop, obj)) {
    pairs[pairs.length] = [prop, obj[prop]];
  }
...
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
...
 * @return {Array} An array of key, value arrays from the object's own
 *         and prototype properties.
 * @example
 *
 *      var F = function() { this.x = 'X'; };
 *      F.prototype.y = 'Y';
 *      var f = new F();
 *      R.toPairsIn(f); //=> [['x','X'], ['y','Y']]
 */
module.exports = _curry1(function toPairsIn(obj) {
var pairs = [];
for (var prop in obj) {
  pairs[pairs.length] = [prop, obj[prop]];
}
return pairs;
...
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
...
 * @category String
 * @sig String -> String
 * @param {String} str The string to upper case.
 * @return {String} The upper case version of 'str'.
 * @see R.toLower
 * @example
 *
 *      R.toUpper('abc'); //=> 'ABC'
 */
module.exports = invoker(0, 'toUpperCase');
...
```

#### <a name="apidoc.element.ramda.transduce"></a>[function <span class="apidocSignatureSpan">ramda.</span>transduce (a0, a1, a2, a3)](#apidoc.element.ramda.transduce)
- description and source-code
```javascript
transduce = function (a0, a1, a2, a3) { return fn.apply(this, arguments); }
```
- example usage
```shell
...
 * @return {*} The final, accumulated value.
 * @see R.reduce, R.reduced, R.into
 * @example
 *
 *      var numbers = [1, 2, 3, 4];
 *      var transducer = R.compose(R.map(R.add(1)), R.take(2));
 *
 *      R.transduce(transducer, R.flip(R.append), [], numbers); //=> [2, 3]
 */
module.exports = curryN(4, function transduce(xf, fn, acc, list) {
  return _reduce(xf(typeof fn === 'function' ? _xwrap(fn) : fn), acc, list);
});
...
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
...
* @since v0.19.0
* @category List
* @sig [[a]] -> [[a]]
* @param {Array} list A 2D list
* @return {Array} A 2D list
* @example
*
*      R.transpose([[1, 'a'], [2, 'b'], [3, 'c']]) //=> [[1, 2, 3], ['a', 'b', 'c']]
*      R.transpose([[1, 2, 3], ['a', 'b', 'c']]) //=> [[1, 'a'], [2, 'b'], [3, 'c']]
*
* If some of the rows are shorter than the following rows, their elements are skipped:
*
*      R.transpose([[10, 11], [20], [], [30, 31, 32]]) //=> [[10, 20, 30], [11, 31], [32]]
* @symb R.transpose([[a], [b], [c]]) = [a, b, c]
* @symb R.transpose([[a, b], [c, d]]) = [[a, c], [b, d]]
...
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
...
 * @return {*}
 * @see R.sequence
 * @example
 *
 *      // Returns 'Nothing' if the given divisor is '0'
 *      safeDiv = n => d => d === 0 ? Nothing() : Just(n / d)
 *
 *      R.traverse(Maybe.of, safeDiv(10), [2, 4, 5]); //=> Just([5, 2.5, 2])
 *      R.traverse(Maybe.of, safeDiv(10), [2, 0, 5]); //=> Nothing
 */
module.exports = _curry3(function traverse(of, f, traversable) {
  return sequence(of, map(f, traversable));
});
...
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
...
 * @since v0.6.0
 * @category String
 * @sig String -> String
 * @param {String} str The string to trim.
 * @return {String} Trimmed version of 'str'.
 * @example
 *
 *      R.trim('   xyz  '); //=> 'xyz'
 *      R.map(R.trim, R.split(',', 'x, y, z')); //=> ['x', 'y', 'z']
 */
module.exports = (function() {
var ws = '\x09\x0A\x0B\x0C\x0D\x20\xA0\u1680\u180E\u2000\u2001\u2002\u2003' +
         '\u2004\u2005\u2006\u2007\u2008\u2009\u200A\u202F\u205F\u3000\u2028' +
         '\u2029\uFEFF';
var zeroWidth = '\u200b';
...
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
...
 * @category Function
 * @sig (...x -> a) -> ((e, ...x) -> a) -> (...x -> a)
 * @param {Function} tryer The function that may throw.
 * @param {Function} catcher The function that will be evaluated if 'tryer' throws.
 * @return {Function} A new function that will catch exceptions and send then to the catcher.
 * @example
 *
 *      R.tryCatch(R.prop('x'), R.F)({x: true}); //=> true
 *      R.tryCatch(R.prop('x'), R.F)(null);      //=> false
 */
module.exports = _curry2(function _tryCatch(tryer, catcher) {
return _arity(tryer.length, function() {
  try {
    return tryer.apply(this, arguments);
  } catch (e) {
...
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
...
* @since v0.8.0
* @category Type
* @sig (* -> {*}) -> String
* @param {*} val The value to test
* @return {String}
* @example
*
*      R.type({}); //=> "Object"
*      R.type(1); //=> "Number"
*      R.type(false); //=> "Boolean"
*      R.type('s'); //=> "String"
*      R.type(null); //=> "Null"
*      R.type([]); //=> "Array"
*      R.type(/[A-z]/); //=> "RegExp"
*/
...
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
...
 * @category Function
 * @sig ([*...] -> a) -> (*... -> a)
 * @param {Function} fn
 * @return {Function}
 * @see R.apply
 * @example
 *
 *      R.unapply(JSON.stringify)(1, 2, 3); //=> '[1,2,3]'
 * @symb R.unapply(f)(a, b) = f([a, b])
 */
module.exports = _curry1(function unapply(fn) {
  return function() {
    return fn(Array.prototype.slice.call(arguments, 0));
  };
});
...
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
...
 *
 *      var takesTwoArgs = function(a, b) {
 *        return [a, b];
 *      };
 *      takesTwoArgs.length; //=> 2
 *      takesTwoArgs(1, 2); //=> [1, 2]
 *
 *      var takesOneArg = R.unary(takesTwoArgs);
 *      takesOneArg.length; //=> 1
 *      // Only 1 argument is passed to the wrapped function
 *      takesOneArg(1, 2); //=> [1, undefined]
 * @symb R.unary(f)(a, b, c) = f(a)
 */
module.exports = _curry1(function unary(fn) {
return nAry(1, fn);
...
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
...
 * @param {Function} fn The function to uncurry.
 * @return {Function} A new function.
 * @see R.curry
 * @example
 *
 *      var addFour = a => b => c => d => a + b + c + d;
 *
 *      var uncurriedAddFour = R.uncurryN(4, addFour);
 *      uncurriedAddFour(1, 2, 3, 4); //=> 10
 */
module.exports = _curry2(function uncurryN(depth, fn) {
return curryN(depth, function() {
  var currentDepth = 1;
  var value = fn;
  var idx = 0;
...
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
...
 *        at index 0 of this array will be added to the resulting array, and the element
 *        at index 1 will be passed to the next call to 'fn'.
 * @param {*} seed The seed value.
 * @return {Array} The final list.
 * @example
 *
 *      var f = n => n > 50 ? false : [-n, n + 10];
 *      R.unfold(f, 10); //=> [-10, -20, -30, -40, -50]
 * @symb R.unfold(f, x) = [f(x)[0], f(f(x)[1])[0], f(f(f(x)[1])[1])[0], ...]
 */
module.exports = _curry2(function unfold(fn, seed) {
var pair = fn(seed);
var result = [];
while (pair && pair.length) {
  result[result.length] = pair[0];
...
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
...
 * @sig [*] -> [*] -> [*]
 * @param {Array} as The first list.
 * @param {Array} bs The second list.
 * @return {Array} The first and second lists concatenated, with
 *         duplicates removed.
 * @example
 *
 *      R.union([1, 2, 3], [2, 3, 4]); //=> [1, 2, 3, 4]
 */
module.exports = _curry2(compose(uniq, _concat));
...
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
...
 * @return {Array} The first and second lists concatenated, with
 *         duplicates removed.
 * @see R.union
 * @example
 *
 *      var l1 = [{a: 1}, {a: 2}];
 *      var l2 = [{a: 1}, {a: 4}];
 *      R.unionWith(R.eqBy(R.prop('a')), l1, l2); //=> [{a: 1}, {a: 2}, {a: 4}]
 */
module.exports = _curry3(function unionWith(pred, list1, list2) {
  return uniqWith(pred, _concat(list1, list2));
});
...
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
...
 * @since v0.1.0
 * @category List
 * @sig [a] -> [a]
 * @param {Array} list The array to consider.
 * @return {Array} The list of unique items.
 * @example
 *
 *      R.uniq([1, 1, 2, 1]); //=> [1, 2]
 *      R.uniq([1, '1']);     //=> [1, '1']
 *      R.uniq([[42], [42]]); //=> [[42]]
 */
module.exports = uniqBy(identity);
...
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
...
 * @category List
 * @sig (a -> b) -> [a] -> [a]
 * @param {Function} fn A function used to produce a value to use during comparisons.
 * @param {Array} list The array to consider.
 * @return {Array} The list of unique items.
 * @example
 *
 *      R.uniqBy(Math.abs, [-1, -5, 2, 10, 1, 2]); //=> [-1, -5, 2, 10]
 */
module.exports = _curry2(function uniqBy(fn, list) {
var set = new _Set();
var result = [];
var idx = 0;
var appliedItem, item;
...
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
...
 * @sig (a, a -> Boolean) -> [a] -> [a]
 * @param {Function} pred A predicate used to test whether two items are equal.
 * @param {Array} list The array to consider.
 * @return {Array} The list of unique items.
 * @example
 *
 *      var strEq = R.eqBy(String);
 *      R.uniqWith(strEq)([1, '1', 2, 1]); //=> [1, 2]
 *      R.uniqWith(strEq)([{}, {}]);       //=> [{}]
 *      R.uniqWith(strEq)([1, '1', 1]);    //=> [1]
 *      R.uniqWith(strEq)(['1', 1, 1]);    //=> ['1']
 */
module.exports = _curry2(function uniqWith(pred, list) {
var idx = 0;
var len = list.length;
...
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
...
 * @param {*}        x           An object to test with the 'pred' function and
 *                               pass to 'whenFalseFn' if necessary.
 * @return {*} Either 'x' or the result of applying 'x' to 'whenFalseFn'.
 * @see R.ifElse, R.when
 * @example
 *
 *      // coerceArray :: (a|[a]) -> [a]
 *      var coerceArray = R.unless(R.isArrayLike, R.of);
 *      coerceArray([1, 2, 3]); //=> [1, 2, 3]
 *      coerceArray(1);         //=> [1]
 */
module.exports = _curry3(function unless(pred, whenFalseFn, x) {
  return pred(x) ? x : whenFalseFn(x);
});
...
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
...
 * @category List
 * @sig Chain c => c (c a) -> c a
 * @param {*} list
 * @return {*}
 * @see R.flatten, R.chain
 * @example
 *
 *      R.unnest([1, [2], [[3]]]); //=> [1, 2, [3]]
 *      R.unnest([[1, 2], [3, 4], [5, 6]]); //=> [1, 2, 3, 4, 5, 6]
 */
module.exports = chain(_identity);
...
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
...
 * @sig (a -> Boolean) -> (a -> a) -> a -> a
 * @param {Function} pred A predicate function
 * @param {Function} fn The iterator function
 * @param {*} init Initial value
 * @return {*} Final value that satisfies predicate
 * @example
 *
 *      R.until(R.gt(R.__, 100), R.multiply(2))(1) // => 128
 */
module.exports = _curry3(function until(pred, fn, init) {
var val = init;
while (!pred(val)) {
  val = fn(val);
}
return val;
...
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
...
 * @param {Number} idx The index to update.
 * @param {*} x The value to exist at the given index of the returned array.
 * @param {Array|Arguments} list The source array-like object to be updated.
 * @return {Array} A copy of 'list' with the value at index 'idx' replaced with 'x'.
 * @see R.adjust
 * @example
 *
 *      R.update(1, 11, [0, 1, 2]);     //=> [0, 11, 2]
 *      R.update(1)(11)([0, 1, 2]);     //=> [0, 11, 2]
 * @symb R.update(-1, a, [b, c]) = [b, a]
 * @symb R.update(0, a, [b, c]) = [a, c]
 * @symb R.update(1, a, [b, c]) = [b, a]
 */
module.exports = _curry3(function update(idx, x, list) {
return adjust(always(x), idx, list);
...
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
...
 * @sig (x1 -> x2 -> ... -> z) -> [(a -> x1), (b -> x2), ...] -> (a -> b -> ... -> z)
 * @param {Function} fn The function to wrap.
 * @param {Array} transformers A list of transformer functions
 * @return {Function} The wrapped function.
 * @see R.converge
 * @example
 *
 *      R.useWith(Math.pow, [R.identity, R.identity])(3, 4); //=> 81
 *      R.useWith(Math.pow, [R.identity, R.identity])(3)(4); //=> 81
 *      R.useWith(Math.pow, [R.dec, R.inc])(3, 4); //=> 32
 *      R.useWith(Math.pow, [R.dec, R.inc])(3)(4); //=> 32
 * @symb R.useWith(f, [g, h])(a, b) = f(g(a), h(b))
 */
module.exports = _curry2(function useWith(fn, transformers) {
return curryN(transformers.length, function() {
...
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
...
 * @since v0.1.0
 * @category Object
 * @sig {k: v} -> [v]
 * @param {Object} obj The object to extract values from
 * @return {Array} An array of the values of the object's own properties.
 * @example
 *
 *      R.values({a: 1, b: 2, c: 3}); //=> [1, 2, 3]
 */
module.exports = _curry1(function values(obj) {
var props = keys(obj);
var len = props.length;
var vals = [];
var idx = 0;
while (idx < len) {
...
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
...
 * @param {Object} obj The object to extract values from
 * @return {Array} An array of the values of the object's own and prototype properties.
 * @example
 *
 *      var F = function() { this.x = 'X'; };
 *      F.prototype.y = 'Y';
 *      var f = new F();
 *      R.valuesIn(f); //=> ['X', 'Y']
 */
module.exports = _curry1(function valuesIn(obj) {
var prop;
var vs = [];
for (prop in obj) {
  vs[vs.length] = obj[prop];
}
...
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
...
 * @param {Function} setter
 * @return {Lens}
 * @see R.view, R.set, R.over, R.lensIndex, R.lensProp
 * @example
 *
 *      var xLens = R.lens(R.prop('x'), R.assoc('x'));
 *
 *      R.view(xLens, {x: 1, y: 2});            //=> 1
 *      R.set(xLens, 4, {x: 1, y: 2});          //=> {x: 4, y: 2}
 *      R.over(xLens, R.negate, {x: 1, y: 2});  //=> {x: -1, y: 2}
 */
module.exports = _curry2(function lens(getter, setter) {
return function(toFunctorFn) {
  return function(target) {
    return map(
...
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
...
 * @sig a -> *
 * @param {*} x The final value of the reduce.
 * @return {*} The wrapped value.
 * @see R.reduce, R.transduce
 * @example
 *
 *      R.reduce(
 *        R.pipe(R.add, R.when(R.gte(R.__, 10), R.reduced)),
 *        0,
 *        [1, 2, 3, 4, 5]) // 10
 */

module.exports = _curry1(_reduced);
...
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
...
* @sig {String: (* -> Boolean)} -> {String: *} -> Boolean
* @param {Object} spec
* @param {Object} testObj
* @return {Boolean}
* @example
*
*      // pred :: Object -> Boolean
*      var pred = R.where({
*        a: R.equals('foo'),
*        b: R.complement(R.equals('bar')),
*        x: R.gt(__, 10),
*        y: R.lt(__, 20)
*      });
*
*      pred({a: 'foo', b: 'xxx', x: 11, y: 19}); //=> true
...
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
...
 * @param {Object} spec
 * @param {Object} testObj
 * @return {Boolean}
 * @see R.where
 * @example
 *
 *      // pred :: Object -> Boolean
 *      var pred = R.whereEq({a: 1, b: 2});
 *
 *      pred({a: 1});              //=> false
 *      pred({a: 1, b: 2});        //=> true
 *      pred({a: 1, b: 2, c: 3});  //=> true
 *      pred({a: 1, b: 1});        //=> false
 */
module.exports = _curry2(function whereEq(spec, testObj) {
...
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
...
 * @sig [a] -> [a] -> [a]
 * @param {Array} list1 The values to be removed from 'list2'.
 * @param {Array} list2 The array to remove values from.
 * @return {Array} The new array without values in 'list1'.
 * @see R.transduce
 * @example
 *
 *      R.without([1, 2], [1, 2, 1, 3, 4]); //=> [3, 4]
 */
module.exports = _curry2(function(xs, list) {
  return reject(flip(_contains)(xs), list);
});
...
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
...
 * @sig [a] -> [b] -> [[a,b]]
 * @param {Array} as The first list.
 * @param {Array} bs The second list.
 * @return {Array} The list made by combining each possible pair from
 *         'as' and 'bs' into pairs ('[a, b]').
 * @example
 *
 *      R.xprod([1, 2], ['a', 'b']); //=> [[1, 'a'], [1, 'b'], [2, 'a'], [2, 'b']]
 * @symb R.xprod([a, b], [c, d]) = [[a, c], [a, d], [b, c], [b, d]]
 */
module.exports = _curry2(function xprod(a, b) { // = xprodWith(prepend); (takes about 3 times as long...)
var idx = 0;
var ilen = a.length;
var j;
var jlen = b.length;
...
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
...
 * @category List
 * @sig [a] -> [b] -> [[a,b]]
 * @param {Array} list1 The first array to consider.
 * @param {Array} list2 The second array to consider.
 * @return {Array} The list made by pairing up same-indexed elements of 'list1' and 'list2'.
 * @example
 *
 *      R.zip([1, 2, 3], ['a', 'b', 'c']); //=> [[1, 'a'], [2, 'b'], [3, 'c']]
 * @symb R.zip([a, b, c], [d, e, f]) = [[a, d], [b, e], [c, f]]
 */
module.exports = _curry2(function zip(a, b) {
var rv = [];
var idx = 0;
var len = Math.min(a.length, b.length);
while (idx < len) {
...
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
...
 * @category List
 * @sig [String] -> [*] -> {String: *}
 * @param {Array} keys The array that will be properties on the output object.
 * @param {Array} values The list of values on the output object.
 * @return {Object} The object made by pairing up same-indexed elements of 'keys' and 'values'.
 * @example
 *
 *      R.zipObj(['a', 'b', 'c'], [1, 2, 3]); //=> {a: 1, b: 2, c: 3}
 */
module.exports = _curry2(function zipObj(keys, values) {
var idx = 0;
var len = Math.min(keys.length, values.length);
var out = {};
while (idx < len) {
  out[keys[idx]] = values[idx];
...
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
...
 * @return {Array} The list made by combining same-indexed elements of 'list1' and 'list2'
 *         using 'fn'.
 * @example
 *
 *      var f = (x, y) => {
 *        // ...
 *      };
 *      R.zipWith(f, [1, 2, 3], ['a', 'b', 'c']);
 *      //=> [f(1, 'a'), f(2, 'b'), f(3, 'c')]
 * @symb R.zipWith(fn, [a, b, c], [d, e, f]) = [fn(a, d), fn(b, e), fn(c, f)]
 */
module.exports = _curry3(function zipWith(fn, a, b) {
var rv = [];
var idx = 0;
var len = Math.min(a.length, b.length);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
