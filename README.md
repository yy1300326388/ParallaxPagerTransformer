[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-ParallaxPagerTransformer-brightgreen.svg?style=flat)](https://android-arsenal.com/details/1/1312)

# ParallaxPagerTransformer

A pager transformer for Android with parallax effect

## Installation

in your build.gradle file

    dependencies {
        // ...
        compile 'com.xgc1986.android:parallaxpagertransformer:1.0.3'
    }

## Usage

minSdkVersion 11

You only have to pass to the ParallaxTransformer the id of the element you want have the parallax effect

```java

	//...
	import com.xgc1986.parallaxPagerTransformer.ParallaxPagerTransformer;

	public class MainActivity extends Activity {

		ViewPager mPager;
    	FragmentStatePagerAdapter mAdapter;

		public void onCreate(Bundle savedInstanceState) {
			/** ... **/

			mPager = (ViewPager) findViewById(R.id.pager);

        	// creating the parallaxTransformer, you only need to pass the id of the View (or ViewGroup) you want to do the parallax effect

        	mPager.setPageTransformer(false, new ParallaxPagerTransformer(R.id.parallaxContent));
        	mAdapter = new FragmentStatePagerAdapter(getSupportFragmentManager());
        	mAdapter.setPager(mPager);

        	/** ... **/
		}
	}

```

And that's all, you can see in action <a href="https://www.youtube.com/watch?v=5zEOUWY9Hvo" target="_blank">Here</a>

## Other works
<a href="https://github.com/xgc1986/RippleButton" target="_blank">Ripple Button</a>

[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-ParallaxPagerTransformer-brightgreen.svg?style=flat)](https://android-arsenal.com/details/1/1312)
