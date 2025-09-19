{\rtf1\ansi\ansicpg949\cocoartf2822
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fnil\fcharset0 Menlo-Regular;\f1\fnil\fcharset129 AppleSDGothicNeo-Regular;\f2\fnil\fcharset0 Menlo-Italic;
}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;\red0\green0\blue0;\red246\green246\blue239;
\red252\green93\blue186;\red238\green252\blue122;\red253\green170\blue90;\red174\green122\blue247;}
{\*\expandedcolortbl;;\cssrgb\c0\c0\c0;\csgray\c0\c0;\cssrgb\c97255\c97255\c94902;
\cssrgb\c100000\c47451\c77647;\cssrgb\c94510\c98039\c54902;\cssrgb\c100000\c72157\c42353;\cssrgb\c74118\c57647\c97647;}
{\*\listtable{\list\listtemplateid1\listhybrid{\listlevel\levelnfc23\levelnfcn23\leveljc0\leveljcn0\levelfollow0\levelstartat1\levelspace360\levelindent0{\*\levelmarker \{none\}}{\leveltext\leveltemplateid1\'00;}{\levelnumbers;}\fi-360\li720\lin720 }{\listname ;}\listid1}
{\list\listtemplateid2\listhybrid{\listlevel\levelnfc23\levelnfcn23\leveljc0\leveljcn0\levelfollow0\levelstartat1\levelspace360\levelindent0{\*\levelmarker \{none\}}{\leveltext\leveltemplateid101\'00;}{\levelnumbers;}\fi-360\li720\lin720 }{\listname ;}\listid2}}
{\*\listoverridetable{\listoverride\listid1\listoverridecount0\ls1}{\listoverride\listid2\listoverridecount0\ls2}}
\paperw11900\paperh16840\margl1440\margr1440\vieww17840\viewh9700\viewkind0
\deftab720
\pard\pardeftab720\partightenfactor0

\f0\fs24 \cf2 \cb3 \expnd0\expndtw0\kerning0
\
#
\f1 \'bb\'e7\'bf\'eb
\f0  
\f1 \'b5\'a5\'c0\'cc\'c5\'cd
\f0  
\f1 \'bc\'b3\'b8\'ed
\f0 \
\
\pard\tx220\tx720\pardeftab720\li720\fi-720\partightenfactor0
\ls1\ilvl0\cf0 \cb1 \kerning1\expnd0\expndtw0 		\expnd0\expndtw0\kerning0
exclusive_use_area : 
\f1 \'bc\'d2\'c0\'af\'c0\'da\'b0\'a1
\f0  
\f1 \'b5\'b6\'c1\'a1\'c0\'fb\'c0\'b8\'b7\'ce
\f0  
\f1 \'bb\'e7\'bf\'eb\'c7\'d2
\f0  
\f1 \'bc\'f6
\f0  
\f1 \'c0\'d6\'b4\'c2
\f0  
\f1 \'b0\'f8\'b0\'a3
\f0 \
\ls1\ilvl0\kerning1\expnd0\expndtw0 		\expnd0\expndtw0\kerning0
transaction_year_month : 
\f1 \'b0\'c5\'b7\'a1
\f0  
\f1 \'bf\'ac\'bf\'f9
\f0 \
\pard\tx220\tx659\tx722\tx811\pardeftab720\partightenfactor0
\ls1\ilvl0\cf0 \kerning1\expnd0\expndtw0 		\expnd0\expndtw0\kerning0
year_of_completion : 
\f1 \'b0\'c5\'b7\'a1\'bf\'cf\'b7\'e1\'bf\'ac\'b5\'b5
\f0 \kerning1\expnd0\expndtw0 	\expnd0\expndtw0\kerning0
\
\pard\tx220\tx720\pardeftab720\li720\fi-720\partightenfactor0
\ls2\ilvl0\cf0 \kerning1\expnd0\expndtw0 		\expnd0\expndtw0\kerning0
transaction_real_price : 
\f1 \'bd\'c7
\f0  
\f1 \'b0\'c5\'b7\'a1
\f0  
\f1 \'b0\'a1\'b0\'dd
\f0 (TARGET)\
\pard\tx720\pardeftab720\partightenfactor0
\cf2 \cb3 \
\
\
\pard\pardeftab720\partightenfactor0
\cf2 ```python\
train = train[['exclusive_use_area', 'transaction_year_month', 'floor', 'year_of_completion', 'transaction_real_price']]\
test = test[['exclusive_use_area', 'transaction_year_month', 'floor', 'year_of_completion']]\
```\
\
```python\
train_x = train.drop('transaction_real_price', 
\f2\i axis
\f0\i0 =1)\
train_y = train['transaction_real_price']\
```}