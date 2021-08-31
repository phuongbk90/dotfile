Erlang

1. Clone asdf

git clone https://github.com/asdf-vm/asdf.git ~/.asdf


2. ZSH

https://www.pluralsight.com/guides/installing-elixir-erlang-with-asdf

https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/asdf

3. Setup
https://www.mashupgarage.com/playbook/setup/asdf.html

asdf plugin-add erlang thtps://github.com/asdf-vm/asdf-erlang.git


https://adoptingerlang.org/docs/development/setup/

sudo apt install gcc-7
asdf global erlang 17.0

// Install openssl
git clone git@github.com:openssl/openssl.git --branch OpenSSL_1_0_2-stable
cd openssl/
mkdir __result
./config --prefix="${HOME}/Downloads/01_Tool/openssl" shared zlib -fPIC
make depend
make
make install INSTALL_PREFIX="${HOME}/Downloads/01_Tool/openssl/__result"

// Export variable
export KERL_CONFIGURE_OPTIONS="--disable-debug --disable-silent-rules --without-javac --enable-shared-zlib --enable-dynamic-ssl-lib --enable-hipe --enable-sctp --enable-smp-support --enable-threads --enable-kernel-poll --enable-wx --with-ssl=${HOME}/Downloads/01_Tool/openssl/__result/${HOME}/Downloads/01_Tool/openssl/"