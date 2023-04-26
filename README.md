# @slise/embed-react

[![npm package][npm-img]][npm-url]
[![Build Status][build-img]][build-url]
[![Downloads][downloads-img]][downloads-url]
[![Issues][issues-img]][issues-url]
[![Code Coverage][codecov-img]][codecov-url]
[![Commitizen Friendly][commitizen-img]][commitizen-url]
[![Semantic Release][semantic-release-img]][semantic-release-url]

> React component to embed Slise into your website

## Install

```bash
npm install @slise/embed-react
```

## Usage

```ts
import { SliseAd } from '@slise/embed-react'

export const App: React.FC = () => {
	return (
		<div>
			<p>Leaderboard example:</p>
			<SliseAd
				style = {{ display: "inline-block", width: "728px", height: "90px" }}
				slotId = "1"
				pub = "pub-12345"
				format = "728x90,364x45"
			/>
		</div>
	)
}
```

## API

### type SliseAdProps

#### slotId

Type: `string`

Unique ID of the slot across all the pages on your website.

#### pub

Type: `string`

Publisher ID (provided by Slise).

#### format

Type: `string`

Comma-separated list of the ad formats that you want to be shown in this slot.

#### style?

Type: `React.CSSProperties`

You can add any valid React CSS styles to the ad.

### SliseAd(props: SliseAdProps)

Displays Slise ad in an iframe.

[build-img]:https://github.com/slisexyz/embed-react/actions/workflows/release.yml/badge.svg
[build-url]:https://github.com/slisexyz/embed-react/actions/workflows/release.yml
[downloads-img]:https://img.shields.io/npm/dt/typescript-npm-package-template
[downloads-url]:https://www.npmtrends.com/typescript-npm-package-template
[npm-img]:https://img.shields.io/npm/v/typescript-npm-package-template
[npm-url]:https://www.npmjs.com/package/typescript-npm-package-template
[issues-img]:https://img.shields.io/github/issues/slisexyz/embed-react
[issues-url]:https://github.com/slisexyz/embed-react/issues
[codecov-img]:https://codecov.io/gh/slisexyz/embed-react/branch/main/graph/badge.svg
[codecov-url]:https://codecov.io/gh/slisexyz/embed-react
[semantic-release-img]:https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg
[semantic-release-url]:https://github.com/semantic-release/semantic-release
[commitizen-img]:https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
[commitizen-url]:http://commitizen.github.io/cz-cli/
