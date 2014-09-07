moodle-editor_atto-chemistry
============================

Chemistry equation editor for Moodle using the mhchem TeX extension in MathJax

Installation

Either

Download the zip file, unzip to give the moodle-atto_editor-chemistry folder. Rename this to chemistry and copy to the lib/editor/atto/plugins directory of your Moodle installation to give lib/editor/atto/plugins/chemistry

Or
Navigate to the lib/editor/atto/plugins directory of your Moodle installation. Then isue the command
git clone https://github.com/geoffrowland/moodle-editor_atto-chemistry.git chemistry.

Then visit the Admin notifications page of your Moodle to complete the installation.

Copy flask.png and flask.svg from chemistry/pix/e/ to the pix/e/ folder of your Moodle installation.

Add chemistry to Administration > Site administration > Plugins > Text editors > Atto HTML editor > Atto toolbar settings > Toolbar config, to give, for example:

insert = chemistry, equation, mathslate, charmap, table, clear

Finally, add mhchem to the Moodle MathJax filter configuration

Edit Administration > Site administration > Plugins > Filters > MathJax > MathJax configuration to include:

TeX: {
  extensions: ["mhchem.js","color.js","AMSmath.js","AMSsymbols.js","noErrors.js","noUndefined.js"]
},

Enjoy!






