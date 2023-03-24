# 2D Accelerated Rendering

'''Include File(s):''' [SDL_render.h](https://github.com/libsdl-org/SDL/blob/main/include/SDL_render.h)


## Introduction
This category contains functions for 2D accelerated rendering.

This API supports the following features:

* single pixel points
* single pixel lines
* filled rectangles
* texture images

All of these may be drawn in opaque, blended, or additive modes.

The texture images can have an additional color tint or alpha modulation applied to them, and may also be stretched with linear interpolation, rotated or flipped/mirrored.

For advanced functionality like particle effects or actual 3D you should use SDL's OpenGL/Direct3D support or one of the many available 3D engines.

This API is not designed to be used from multiple threads, see [SDL issue #986](https://github.com/libsdl-org/SDL/issues/986) for details.

<!-- BEGIN CATEGORY LIST -->
- [SDL_BlendFactor](SDL_BlendFactor)
- [SDL_BlendOperation](SDL_BlendOperation)
- [SDL_ComposeCustomBlendMode](SDL_ComposeCustomBlendMode)
- [SDL_CreateRenderer](SDL_CreateRenderer)
- [SDL_CreateSoftwareRenderer](SDL_CreateSoftwareRenderer)
- [SDL_CreateTexture](SDL_CreateTexture)
- [SDL_CreateTextureFromSurface](SDL_CreateTextureFromSurface)
- [SDL_CreateWindowAndRenderer](SDL_CreateWindowAndRenderer)
- [SDL_DestroyRenderer](SDL_DestroyRenderer)
- [SDL_DestroyTexture](SDL_DestroyTexture)
- [SDL_GetNumRenderDrivers](SDL_GetNumRenderDrivers)
- [SDL_GetRenderDrawBlendMode](SDL_GetRenderDrawBlendMode)
- [SDL_GetRenderDrawColor](SDL_GetRenderDrawColor)
- [SDL_GetRenderer](SDL_GetRenderer)
- [SDL_GetRendererInfo](SDL_GetRendererInfo)
- [SDL_GetRenderTarget](SDL_GetRenderTarget)
- [SDL_GetTextureAlphaMod](SDL_GetTextureAlphaMod)
- [SDL_GetTextureBlendMode](SDL_GetTextureBlendMode)
- [SDL_GetTextureColorMod](SDL_GetTextureColorMod)
- [SDL_GL_BindTexture](SDL_GL_BindTexture)
- [SDL_GL_UnbindTexture](SDL_GL_UnbindTexture)
- [SDL_LockTexture](SDL_LockTexture)
- [SDL_QueryTexture](SDL_QueryTexture)
- [SDL_RenderClear](SDL_RenderClear)
- [SDL_Renderer](SDL_Renderer)
- [SDL_RendererFlags](SDL_RendererFlags)
- [SDL_RendererFlip](SDL_RendererFlip)
- [SDL_RendererInfo](SDL_RendererInfo)
- [SDL_RenderFillRect](SDL_RenderFillRect)
- [SDL_RenderFillRects](SDL_RenderFillRects)
- [SDL_RenderGeometry](SDL_RenderGeometry)
- [SDL_RenderGeometryRaw](SDL_RenderGeometryRaw)
- [SDL_RenderPresent](SDL_RenderPresent)
- [SDL_RenderReadPixels](SDL_RenderReadPixels)
- [SDL_SetRenderDrawBlendMode](SDL_SetRenderDrawBlendMode)
- [SDL_SetRenderDrawColor](SDL_SetRenderDrawColor)
- [SDL_SetRenderTarget](SDL_SetRenderTarget)
- [SDL_SetTextureAlphaMod](SDL_SetTextureAlphaMod)
- [SDL_SetTextureBlendMode](SDL_SetTextureBlendMode)
- [SDL_SetTextureColorMod](SDL_SetTextureColorMod)
- [SDL_Texture](SDL_Texture)
- [SDL_TextureAccess](SDL_TextureAccess)
- [SDL_TextureModulate](SDL_TextureModulate)
- [SDL_UnlockTexture](SDL_UnlockTexture)
- [SDL_UpdateTexture](SDL_UpdateTexture)
- [SDL_UpdateYUVTexture](SDL_UpdateYUVTexture)
<!-- END CATEGORY LIST -->

----
[CategoryCategory](CategoryCategory)

